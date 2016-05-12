## This is a simple slider for images to be used in a Wordpress website.
It creates an infinite automatic horizontal looping.

To use this application, add the html with the images to your WordPress page.

Add the slider-style css to your main css stylesheet (style.css)

Enqueue the javascript in your functions.php file using:

```

add_action( 'wp_enqueue_scripts', 'slider_scripts' );
function slider_scripts() {
  wp_enqueue_script( 'logo-slider-js', get_stylesheet_directory_uri() . '/js/logo-slider.js', array( 'jquery' ), '1.2', true );
}
```

