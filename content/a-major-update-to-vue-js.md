---
title: A Major Update to VueJS
image:
imageMeta:
  attribution:
  attributionLink:
featured: true
authors: 
  - luke
date: Sat Jan 29 2022 15:11:53 GMT+1100 (Australian Eastern Daylight Time)
tags:
  - new
---

My thought process on updating from VueJS 2 to VueJS 3.

# Why update?

VueJS 3 has many new and improved features, for example the new composition API,
new rendering engine etc. It can even allow sibling elements, so we no longer have
wrap components in a div container.

An update has also given us the opportunity to remove any components that are no longer
being maintained. We have gone through all our code and have started removing certain
components. We have replaced these components with another library which is currently
being supported. Example would be the datetime picker, and the vueselect (which is not
supported on VueJS 3).

# What else is being updated?

Excluded the above mentioned componenets, we are also updating our code to enable
lazy loading. We are hoping this feature will help those who are on slow internet,
only load up exactly what they are using and nothing else. For example, the parent
module at the bottom of Project Information page, has many tabs with many different
components installed. If the user does not navigate to any of the tabs, why are we
loading up those components? We are hoping that the lazy load feature coupled with
other features in VueJS 3, will allow us to only load that component when it is
required.

Another year programming VueJS has passed, and I have gotten better at coding VueJS.
From this understanding I have noticed that there are some bad code here and there.
I intend to fix this as I am re-writing for VueJS 3. The idea behind this is so if
there are others who want to contribute to NearBeach, the code will be easier for them
to read, pickup, and contribute.


# Issues and recommendations

### Components are not supported in VueJS 3

We have come across a few components that are not yet supported in VueJS 3. These
components have had to be stripped out of NearBeach and replaced with an
equivalent. This does take time.

There is nothing you can do in these cases, as we can not predict libraries and 
components not being supported in Major version in the future. In some cases they do
however they themselfs need major updates also. We came across this issue when dealing
with the Vue Draggable. It was supported in VueJS 3, however we needed to update the
code surrownding this component.

### Patience & Time

Everything will break when a MAJOR update occurs. The only thing that can fix this is
patience and time. After the initial fixes have been implemented, we then need to go
back and test the whole application over and over again.

I was hoping to have this finished by Jan 20th - but I missed that timeline sadly.
