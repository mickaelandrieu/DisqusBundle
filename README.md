Disqus Bundle
===================


This bundle add Disqus Comment service integration to BackBee CMS.

----------


## Installation

Use composer to require the Bundle:

```php
$~ composer require "mickaelandrieu/disqus-bundle:1.0"
```

Then, register the bundle in `bundles.yml`:

```yaml
# bundles configuration, in repository/Config/bundles.yml
demo: BackBee\Bundle\DemoBundle\Demo
toolbar: BackBee\Bundle\ToolbarBundle\Toolbar
# ...
disqus: Am\Bundle\DisqusBundle\Disqus
```

Finaly, you need to set up your [Disqus Application short name](https://help.disqus.com/customer/portal/articles/466208).


```yaml
# in repository/Config/services.yml
parameters:
    bundle.disqus.short_name: disqus_application_name
```

You can know access the new block "Disqus" in "Comment" category.

![Disqus Block Comment](http://i.imgur.com/WENzTKR.png)


