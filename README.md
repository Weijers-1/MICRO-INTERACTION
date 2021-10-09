# Micro Interaction
Micro Interaction is an easy way to trigger animations once your website visitors are able to see an element.

## Example
```html
<!DOCTYPE html>
<html>
  <head>
    <title>My cool site</title>
    <link rel="stylesheet" href="https://open-source.extive.eu/micro-interaction-theme.css" type="text/css">
    <script src="https://open-source.extive.eu/micro-interaction.js" type="text/javascript"></script>
    <style type="text/css">
      .some-white-space{
        position: relative;
        height: 100vh;
        width: 100vw;
      }
    </style>
  </head>
  <body>
    <div class="some-white-space"></div>
    <div class="animate fadeBottom">
      <h1>Wow! This is an animation!</h1>
    </div>
    <script type="text/javascript">
      new Interact({
        target: 'animate', // Selects all elements with the classname 'animate'
        className: 'animation', // Gives all elements with the classname 'animate' the classname 'animation' once the element is visible for the user
        mobile: false, // Disables the Micro Interaction on phone
        offset: 20, // Starts the animation 20px earlier than the user can see
        reset: false // Disables the replaying the animations
      });
    </script>
  </body>
</html>
```

[Full documentations](https://open-source.extive.eu/micro-interaction)
