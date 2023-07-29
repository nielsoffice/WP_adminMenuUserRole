# WP_adminMenuUserRole
WordPress admin menu hook and user role. check if user role is === 'subscriber' then redirect to the dashboard once clicking the plugin menu or hide menu as well

```PHP
// Hide and redirect page once user having no role to access the menu 
 
 admin_menu();
 remove_menu_page();
 remove_menu_sub_page(); 

 //Check user role 
 $user = wp_get_current_user();
 if ( in_array( 'author', (array) $user->roles ) ) {
    //The user has the "author" role
 }

```

<br /> Source : 
<br /> https://wordpress.stackexchange.com/questions/5047/how-to-check-if-a-user-is-in-a-specific-role
