---
layout: post
title:  "Some Thoughts of AngularJs"
date:   2016-01-17 19:15:58 +0800
remark: Javascript
author: Andrew Wu
comments: true
categories: javascript
---

I'm still quite new to the AngularJS, but with my recent experience, I've found something quite exciting.

2-way data binding is definitely something worth talking about, it has both pros and cons. Since I've just switched to 
AngularJS from jQuery, one very obvious advantage is that I no longer need to do tedious dirty checking manually to 
monitor all the inputs and data. Angular does it for me with just one in-line attribute, which is `ng-model`. And with 
ng-model, I am allowed to link multiple inout fields together to get the form data. But there are negative sides as 
well, inputs and ng-model are of one-to-one relationship, that means we can neither have a composite ng-model which 
crosses multiple inputs nor a input that binds multiple ng-models. Compared to jQuery, angularJS has made things 
much easier in terms of change-checking and event-triggering, but when it comes to single element support, I feel that 
jQuery has offered more flexibility than Angular.
 
One of other nice things to have is `$scope`, together with directive, it helps a lot in modelization. Besides, $scope 
allows a very convenient access to certain element. Moreover, most of the angular expression uses in-line `ng` attribute 
to achieve dynamic, this kind of keyword defining saves a lot of efforts in coding line by line to achieve same effects 
than jQuery. 

Some other things like `$routeProvider`, `$stateProvider` are also very useful for different circumstances. However, I'm 
still exploring this framework. Hopefully I will find out more soon.