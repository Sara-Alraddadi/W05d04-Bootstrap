# W05d04-Bootstrap
[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)

# Bootstrap 
<br>

## Why is this important?
<!-- framing the "why" in big-picture/real world examples -->
*This workshop is important because:*

Bootstrap is a **library of CSS classes** that helps make any old site look nice with very little effort. It comes with a **grid system** that makes layout out content on a variety of screen sizes much easier to deal with. Proficiency in at least one CSS framework allows you to make better first impressions when people land on your page.



## Where should we be now?
<!-- call out the skills that are prerequisites -->
*Before this workshop, developers should already be able to:*

- Write custom HTML & CSS
- Include external stylesheets



## Intro to Bootstrap
![bootstrap example](https://upload.wikimedia.org/wikipedia/commons/thumb/6/66/Twitter_Bootstrap_Under_Firefox_32.png/1200px-Twitter_Bootstrap_Under_Firefox_32.png)

* [Bootstrap](http://getbootstrap.com/) is a **CSS framework** created by a small team of developers at Twitter and maintained by a much larger community of contributors.
* The framework consists of one main CSS file, an optional theme CSS file, and a main JS file.
* Parts of Bootstrap require [jQuery](https://code.jquery.com/) to work.
* To apply bootstrap styles, you just add classes to your HTML elements. The Bootstrap CSS files style these classes in complex ways.
* It has excellent documentation!

Bootstrap comes with a ton of features, including:

- [Responsive Grid System](https://getbootstrap.com/docs/4.0/examples/grid/)
- CSS library for quick and easy styling
- UI components - HTML + CSS
  - buttons
  - forms
  - etc.
- Javascript widgets to make your page interactive (e.g. a nav bar)
- Icons
- & more!

## Notable Sites Using Bootstrap

* [NBA.com](http://www.nba.com/)
* [Bloomberg](http://www.bloomberg.com/)
* [CodeAcademy](https://www.codecademy.com/)



## For a complete list of features :  

[Bootstrap](http://getbootstrap.com/)



# Install Bootstrap
## Add bootstrap to your Gemfile:
```
gem 'bootstrap-sass', '~> 3.3.6'
gem 'bootstrap', '~> 4.4.1'

```
```
gem install bundler
bundle install
```
 go to app/assets/stylesheets/application.scss 
 Make sure the file has .scss extension 

 > SCSS is a special type of file for SASS, a program written in Ruby that assembles CSS style sheets for a browser. SASS adds lots of additional functionality to CSS like variables, nesting and more which can make writing CSS easier and faster
```
@import "bootstrap-sprockets";
@import "bootstrap";
```
> Imports allow you to include HTML documents within other HTML documents 

add the jquery-rails gem to your Gemfile:
```
gem 'jquery-rails'
```
```
bundle install
```

Add Bootstrap dependencies and Bootstrap to your application.js in javascript folder:
```
//= require jquery3
//= require popper
//= require bootstrap-sprockets
```
## restart your server


# Now lets add some styles 


go to ```index-html-erb``` add class ```table``` to your table tag

add class ```table-hover``` for more stylish table 

add class ```display-3 text-center`` to your heading

add at the top 
```
<div class = "container-fluid" style="background-color: black;">
<ul class="nav nav-pills nav-justified">
  <li class="nav-item">
    <a class="nav-link active" href="/">Muse</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="/artists/new">Create New Artist</a>
  </li>
 
 
</ul>
</div>
```
wrap the rest of the elements in 
```
<div class = "container">

</div>
```

# Now lets add some icons

open https://getbootstrap.com/docs/3.3/components/

replace to this class  ```"glyphicon glyphicon-edit"``` in anchor tag
and remove <i> tag

replace to this class  ```"glyphicon glyphicon-trash"``` in anchor tag
and remove <i> tag





## Helpful References

http://getbootstrap.com/components/

http://getbootstrap.com/css/

http://getbootstrap.com/customize/

https://github.com/twbs/bootstrap-sass

http://www.tutorialspoint.com/bootstrap/

http://bootsnipp.com/

http://tutorialzine.com/2015/06/12-time-saving-bootstrap-examples/

http://builtwithbootstrap.com/

https://bootstrapbay.com/blog/built-with-bootstrap/

## Additional Resources

- [Foundation](http://foundation.zurb.com/) - another CSS-library, similar to Bootstrap
- [Skeleton](http://getskeleton.com/) - a lovely, minimal, unopinionated CSS library
- [Materialize](http://materializecss.com/) - front-end framework based on "material design"
- [Block Element Modifier methodology](http://getbem.com/introduction/)
- [Hipster Ipsum](http://hipsum.co/) - Dummy placeholder "hipster" text
