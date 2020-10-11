# wordpress-to-many-redirect
wordpress to many redirect solutions 

Add this code in  wp-config.php after <?php

    if ( isset( $_SERVER['HTTP_X_FORWARDED_PROTO'] ) && 'https' == $_SERVER['HTTP_X_FORWARDED_PROTO'] ) {
        $_SERVER['HTTPS'] = 'on';
    }
