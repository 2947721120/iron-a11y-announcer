
<!---

This README is automatically generated from the comments in these files:
iron-a11y-announcer.html

Edit those files, and our readme bot will duplicate them over here!
Edit this file, and the bot will squash your changes :)

-->

[![构建状态](https://travis-ci.org/PolymerElements/iron-a11y-announcer.svg?branch=master)](https://travis-ci.org/PolymerElements/iron-a11y-announcer)

_[Demo and API Docs](https://elements.polymer-project.org/elements/iron-a11y-announcer)_


##&lt;iron-a11y-announcer&gt;


`iron-a11y-announcer` 是为了增加A11Y到需要按需宣布从屏幕阅读器功能的单元素。为了充分利用播音员的，最好是在宣布元素要求其可用性。

例子:

    Polymer({

      is: 'x-chatty',

      attached: function() {
     //这将创建单元素，如果它没有被创建//尚未：
        Polymer.IronA11yAnnouncer.requestAvailability();
      }
    });

之后 `iron-a11y-announcer` 已提供，元件可通过烧制鼓泡使日公布 `iron-announce` events.

Example:

    this.fire('iron-announce', {
      text: 'This is an announcement!'
    }, { bubbles: true });

Note: announcements are only audible if you have a screen reader enabled.


