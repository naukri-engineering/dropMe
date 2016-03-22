DropMe Plugin
============================
DropMe provides drag and drop features for html elements using jquery.

DEMO
============================
[Click Me for Demo:](http://naukri-engineering.github.io/dropMe/)
-------------------------------------------------------

## Browser Support
* Internet Explorer 8+
* Chrome 10+
* Firefox 3.5+
* Safari 4+
* Opera 11+

-------------------------------------------------------
## Size
* Less than 1KB

-------------------------------------------------------

Usage
-----
For List with Object to insert data
var options = {
	contId:'ID to insert list',
	elem:[{id:1,title:'nitin'},{id:2,title:'ankit'},{id:3,title:'himanshu'},{id:4,title:'prashu'}]
	}
$('.dropme').dropme(options);
-----
Use `dropme` method to create a draggable list:

``` javascript
$('.dropme').dropme();
```

Use `sortupdate` event if you want to do something when the order changes:

``` javascript
$('.dropme').dropme().bind('sortupdate', function(e, elm) {
    //Triggered when the position has changed.
});
```

Use `items` option to specifiy which items inside the element should be sortable:

``` javascript
$('.dropme').dropme({
    items: ':not(.disabled)'
});

```
Setting 'replacerSize' option to true, forces the placeholder to have a height:

``` javascript
$('.dropme').dropme({
    replacerSize: true 
});
```

Use `linkTo` option to create connected lists:

``` javascript
$('#id1,#id2').dropme({
    linkTo: '.connected'
});
```

To remove the sortable functionality completely:

``` javascript
$('.dropme').dropme('destroy');
```

To disable the sortable temporarily:

``` javascript
$('.dropme').dropme('disable');
```

To enable a disabled sortable:

``` javascript
$('.dropme').dropme('enable');
```

-------------------------------------------------------

LICENSE
-------
Please see [LICENSE.md](LICENSE.md) for detail


-------------------------------------------------------

Author
------
Nitin Giri