# Navigation-Graph

## -Intro to Navigation Graph 


### -Setting Destination for Nav graph

                    val navHostFragment =
                        supportFragmentManager.findFragmentById(R.id.nav_host) as NavHostFragment
                    val graphInflater = navHostFragment.navController.navInflater
                    val navGraph = graphInflater.inflate(R.navigation.nav_flow)
                    val navController = navHostFragment.navController
                    val destination =  R.id.startingFragment 
                    navGraph.startDestination = destination
                    navController.graph = navGraph


