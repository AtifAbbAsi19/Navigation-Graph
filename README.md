# Navigation-Graph

## -Intro to Navigation Graph 


 <androidx.fragment.app.FragmentContainerView
            android:id="@+id/nav_host"
            android:name="androidx.navigation.fragment.NavHostFragment"
            android:layout_width="0dp"
            android:layout_height="0dp"
            app:defaultNavHost="true"
            android:background="@color/darkBlack"
            app:layout_constraintBottom_toBottomOf="parent"
            app:layout_constraintEnd_toEndOf="parent"
            app:layout_constraintStart_toStartOf="parent"
            app:layout_constraintTop_toBottomOf="@id/toolBarHeader" />



### -Setting Destination for Nav graph

                    val navHostFragment =
                        supportFragmentManager.findFragmentById(R.id.nav_host) as NavHostFragment
                    val graphInflater = navHostFragment.navController.navInflater
                    val navGraph = graphInflater.inflate(R.navigation.nav_flow)
                    val navController = navHostFragment.navController
                    val destination =  R.id.startingFragment 
                    navGraph.startDestination = destination
                    navController.graph = navGraph


