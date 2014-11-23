juliadroid-app
==============

The JuliaDroid app, for Android. It uses the [JuliaDroid](https://github.com/rudimk/juliadroid-backend) backend to allow quick Julia computing, on the go. The app simply passes Julia expressions entered by the user to the backend, which executes them in a Julia instance, and passes the results back as a JSON object.

The app itself, is built using the [Intel XDK](https://software.intel.com/en-us/html5/tools). Why Android? Because this app was built as part of a 5-hour, nocturnal pizza-plus-Tzinga-fuelled session at the Hacknight for [Droidcon India 2014](http://droidcon.in) - and unfortunately, all I have is a sucky Android phone. Why a cross-platform tool like the XDK, and not a native app? Because I'm not much of a mobile app guy, the prospect of coding in Java isn't something I particularly relish, and I needed to build something real quick, or it would have never happened. Of course, this means you need the Intel XDK installed on your dev machine, if you want to hack on this app - which isn't much of an app, by the way. But installing the XDK isn't too complicated, so you'll be alright. Apart from that, you will need working instances of Julia, and the JuliaDroid backend - installing that, again, isn't too complicated. Once everything's set up, all you have to do is fire up the XDK and import this codebase in, and you're set.

While this app's just a prototype, I have some features in mind I'd like to add soon enough, like:

* Adding a nice editor with Julia syntax highlighting; then one can run Julia scripts.
* Migrating from Intel's XDK to something like [Famo.us](https://famo.us/).
* Adding support for SVG plots.
* Integrating user auth between this app and the backend, as well as tracking what expressions were entered, memory consumed on the backend, that sort of thing.
