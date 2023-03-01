# nav-plugin
nav-plugin插件

这是一款用于收集项目中所有Activity、Fragment页面的 gradle 插件，配合jetpack navigation框架使用

Eaxmple:

step1:
@NavDestination(type=NavType.Fragment,route="home_fragment")
class HomeFragment:Fragment{

}
@NavDestination(type=NavType.Activity,route="home_activity")
class HomeActivity:FragmentActivity{

}

step2:
class MainActivity : FragmentActivity{

  fun onCreate(bundle:Bundle){
     NavRegistry.DESTINATIONS
  }
}
