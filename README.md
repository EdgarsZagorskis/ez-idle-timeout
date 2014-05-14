# JS Idle Timeout as a PolymerProject WebComponent

[Demo](https://github.com/EdgarsZagorskis/ez-idle-timout)

Place a HTML text with redirect to URL that happens on idle timeout. Javascript implementation of user idle timout in Polymer Project

## Initialize Polymer Platform

    <script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.2.3/platform.js"></script>
    <script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.2.3/polymer.js"></script>

## Include component

    <ez-idle-timeout  url="/" timewarn="5" timeidle="25">
        Hey, if you have been idle for 5 seconds. If you don't interact with website, you will be redirected to / in 20 seconds
    </ez-idle-timeout>

## How much time remains?

It is possible to fetch the timer along with other timestamps.

To access timer in global space, add attribute "interactive" (we normally don't want to polute global scope, right?)

    <ez-idle-timeout  url="/" timewarn="5" timeidle="25" interactive>
        Now i am accessible from javascript through window.ezIdleTimeout object
    </ez-idle-timeout>

## Share, fork, contribute! :D
pleeeease
