# Notification plugin

**_Notify_** is a minimalist and easy to use notification pluging.  <br/>
Uses only javascript, html and css.

## Getting Started

Add the things described below to your code.

### Head section

First thing is to link javascrip and css plik in your head section.

```
    <link rel="stylesheet" href="css/notification.css"/>
    <script type="text/javascript" src="js/notify.js> </script>
```

### Body section
Next step you have to do if you want use Notify is to add buttons (with the class that is written below) in your body section.

```
          <button class="buttons__success">
            Show (success)
          </button>
          
          <button class="buttons__error">
            Show (error)
          </button>
```

## Usage
The notification will disappear after 10 seconds. <br/>
You can specify type of notification, title and message you want to show.


```
    successBtn.addEventListener("click", () => {
      notify.addNotification({
          type: "success",
          title: "Success!",
          message: "Your notification is working!"
      });
    });
    
    errorBtn.addEventListener("click", () => {
       notify.addNotification({
          type: "error",
          title: "Error!",
          message: "Please try again!"
        }); 
    });

```
