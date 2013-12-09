# Real Time Rack

At least since node.js everyone knows that real time HTTP responses are the
next big thing. The secrets of handling incoming requests asynchronously with
Ruby is not yet far spread among Rubyists, as the internals needed for such
responses are neither specified nor documented and there is a lack of tools.
Still, it is possible to use Server-Sent Events, WebSockets and akin with Rack
today. This talk will demonstrate the underlying technologies and how to use
them in your Ruby application.

### Original Notes

I want to give a talk about real time responses and Rack. This involves
combining streaming and asynchronous events. I feel that this topic is nowhere
covered in depth and knowledge can only be achieved by source code reading and
experimenting, both things I have done intensively. While doing so, I myself
created a library called async-rack, even though my talk will not be about
that project, since it is only of use if you already know how to send async
responses with Rack. The tools and examples demonstrated should easily be
usable with any Rack-based framework, like Rails and Sinatra and therefore be of general interest to most Ruby developers.

I will start with a little teaser: A WebSockets live demo.

After giving a short reminder of what Rack is, I will explain streaming with
Rack. The usual streaming approach does not work on evented servers, like
Thin. At this point, I cover the event loop and why it prevents streaming. I
will go into detail on how to use `async.callback` on servers that do support
it in order to achieve the same functionality without even blocking the event
loop. Based on that I go into details about Server Sent Events (EventSource),
which are far easier to implement and use than WebSockets. And finally, I will
cover WebSockets. If there is enough time left, I will go into deploying such
an application.

My plans are to show a lot of small code snippets and leave the audience at a
point where they could start writing async web applications right away. I will
use a modified version of show-off for giving my presentation, which will run
any demos I'll be giving embedded in the presentation, thus making the overall
presentation both smooth and fun.
