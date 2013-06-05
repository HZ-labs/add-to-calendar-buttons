# OuiCal

A simple JS script that enables you to add an "add to calendar" button to your events.

Call 'createAddToCalendarLinks' with your event info, pass in any optional parameters such as a class and/ or id and boom! Insert your add-to-calendar div wherever you'd like.

The only fields that are mandatory are:

  - Start time
  - End time (or event duration, in minutes)
  - Event tile

## Example

    createAddToCalendarLinks({
      options: {
        class: 'my-class',
        id: 'my-id'
      },
      data: {
        // Event title
        title: 'Billiard And Drinks',

        // Event start date
        start: new Date('June 15, 2013 19:00'),

        // Event duration (IN MINUTES)
        duration: 120,

        // You can also choose to set an end time. 
        // If an end time is set, this will take precedence over duration.
        end: new Date('June 15, 2013 23:00'),

        // Event Address
        address: '714 Moon Street, New York',

        // Event Description
        description: 'Get together with coworkers and shoot some pool.'
      }
    });

[Here is the live example](http://carlsednaoui.github.io/ouical/example.html)

## GitHub Project Page
[Official Project Page](http://carlsednaoui.github.io/ouical/)

## TODO
  - Force user to provide a unique ID for each calendar. Use this ID for both the label and returned DIV.

## License
[MIT](http://opensource.org/licenses/MIT)