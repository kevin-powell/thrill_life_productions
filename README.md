Thrill Life Productions

First steps:
1. install node.js vs 6.11.
    npm vs 3.10.10
2. install bower
3. Terminal: npm install -g bower


Install Bootstrap in your Node powered apps with the npm package:

4. Terminal: npm install bootstrap@4.0.0-alpha.6

5. create a folder scss / within that folder create vendor folder

5. Going to Customize our bootstrap scss:
 a. go to  bower_components/bootstrap
 b. pull out _custom.scss & bootstrap.scss
 c. place these in your vendor folder


 6. Goto bootstrap.scss (only common out what you will be using)
 add to these files
 "../..bower_components/bootstrap/scss/"

 // Core variables and mixins
 @import "custom";
 @import "../../bower_components/bootstrap/scss/variables";
 @import "../../bower_components/bootstrap/scss/mixins";


 // Reset and dependencies
 @import "../../bower_components/bootstrap/scss/normalize";
 @import "../../bower_components/bootstrap/scss/print";

 // Core CSS
 @import "../../bower_components/bootstrap/scss/reboot";
 @import "../../bower_components/bootstrap/scss/type";
 @import "../../bower_components/bootstrap/scss/images";
 //@import "../../bower_components/bootstrap/scss/code";
 @import "../../bower_components/bootstrap/scss/grid";
 //@import "../../bower_components/bootstrap/scss/tables";
 //@import "../../bower_components/bootstrap/scss/forms";
 @import "../../bower_components/bootstrap/scss/buttons";

 // Components
 @import "../../bower_components/bootstrap/scss/transitions";
 //@import "../../bower_components/bootstrap/scss/dropdown";
 //@import "../../bower_components/bootstrap/scss/button-group";
 //@import "../../bower_components/bootstrap/scss/input-group";
 //@import "../../bower_components/bootstrap/scss/custom-forms";
 @import "../../bower_components/bootstrap/scss/nav";
 @import "../../bower_components/bootstrap/scss/navbar";
 @import "../../bower_components/bootstrap/scss/card";
 //@import "../../bower_components/bootstrap/scss/breadcrumb";
 //@import "../../bower_components/bootstrap/scss/pagination";
 //@import "../../bower_components/bootstrap/scss/badge";
 //@import "../../bower_components/bootstrap/scss/jumbotron";
 //@import "../../bower_components/bootstrap/scss/alert";
 //@import "../../bower_components/bootstrap/scss/progress";
 //@import "../../bower_components/bootstrap/scss/media";
 //@import "../../bower_components/bootstrap/scss/list-group";
 @import "../../bower_components/bootstrap/scss/responsive-embed";
 //@import "../../bower_components/bootstrap/scss/close";

 // Components w/ JavaScript
 //@import "../../bower_components/bootstrap/scss/modal";
 //@import "../../bower_components/bootstrap/scss/tooltip";
 //@import "../../bower_components/bootstrap/scss/popover";
 //@import "../../bower_components/bootstrap/scss/carousel";

 // Utility classes
 @import "../../bower_components/bootstrap/scss/utilities";

7. Inside your vendor folder- create a file main.scss
    @import 'abstracts/variables';


    //bring Bootstrap
    @import 'vendor/bootstrap';
    @import 'base/typography';

    @import 'components/navigation';
    @import 'pages/home';

8. In your SCSS folder create
  _home.scss
  abstracts /file: _variables.scss
  base /file: _typography.scss
  components /file: _navigation.scss
  layout
  pages /file: _home.scss

9. Inside thrill_life_productions - create a file
    thrill_index.html

10.  <!-- starter template -->  

<!DOCTYPE html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/css/bootstrap.min.css" integrity="sha384-rwoIResjU2yc3z8GV/NPeZWAv56rSmLldC3R/AZzGRnGxQQKnKkoFVhFQhNUwEyJ" crossorigin="anonymous">
  </head>
  <body>
    <h1></h1>

    <!-- jQuery first, then Tether, then Bootstrap JS. -->
    <script src="https://code.jquery.com/jquery-3.1.1.slim.min.js" integrity="sha384-A7FZj7v+d/sdmMqp/nOQwliLvUsJfDHW+k9Omg/a/EheAdgtzNs3hpfag6Ed950n" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/tether/1.4.0/js/tether.min.js" integrity="sha384-DztdAPBWPRXSA/3eYEEUWrWCy7G5KFbe8fFjk5JAIxUYHKkDx6Qin1DkWx51bBrb" crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/js/bootstrap.min.js" integrity="sha384-vBWWzlZJ8ea9aCX4pEW3rVHjgjt7zpkNpZk+02D9phzyeVkE+jo0ieGizqPLForn" crossorigin="anonymous"></script>
  </body>
</html>

11. Inside thrill_life_productions - create a folder
    fonts
    a. goto fonts http://fontawesome.io/
    b. download
    c. grab zip file font-awesome-4.7.0 and drag to fonts folder
    d. In the <head> of your html, reference the location to your font-awesome.min.css. paste this link
    <link rel="stylesheet" href="path/to/font-awesome/css/font-awesome.min.css">

    e. change link to say:
    <link rel="stylesheet" href="fonts/font-awesome/css/font-awesome.min.css">

    f. fa-calendar-o -  Unicode: f133
    <i class="fa fa-calendar-o" aria-hidden="true"></i>
