## Varnish 3.0 for Drupal 7.x

Intended for use with the varnish, purge, and expires modules.

As per the documentation on drupal.org/project/varnish you should add something like the following to your settings.php file:
  $conf['cache_backends'] = array('sites/all/modules/contrib/varnish/varnish.cache.inc');
  $conf['cache_class_cache_page'] = 'VarnishCache';
  $conf['page_cache_invoke_hooks'] = FALSE;
  $conf['omit_vary_cookie'] = true;

