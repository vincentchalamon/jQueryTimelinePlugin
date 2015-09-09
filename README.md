# jQueryTimelinePlugin

This jQuery plugin allows you to create a timeline.

![](http://www.vincent-chalamon.fr/content/images/2015/04/jquery-timeline.png)

# How to use

This plugin requires [jQuery 1.8+](http://jquery.com/) :
```html
<script type="text/javascript" src="http://code.jquery.com/jquery-1.10.1.min.js"></script>
<script type="text/javascript" src="path/to/jquery.timeline.js"></script>
<link type="text/css" rel="stylesheet" media="screen" href="path/to/timeline.css" />
```

Now you can use jQuery timeline plugin as following :
```javascript
$(function () {
    $('#timeline').timeline({
        elements: [
            {
                start: '2006-09-01',
                end: '2008-08-31',
                css: 'jquery-timeline-item-foo',
                label: 'Lorem ipsum'
            },
            {
                start: '2007-03-12',
                end: '2007-04-14',
                label: 'Dolor sit amet'
            },
            {
                start: '2007-07-01',
                end: '2007-07-31',
                label: 'Foo'
            },
            {
                start: '2008-04-14',
                end: '2008-07-31',
                label: 'Bar'
            }
        ],
        onSelect: function(event, index){
            // Do some stuff
        }
    });
});
```

# Options

You must set following options to timeline :

* elements : array of elements to create
    * start : element start date (string or Date object)
    * end : optional element end date (string or Date object)
    * label : element label
    * css : optional element additional class name
* onSelect : callback on click on item
