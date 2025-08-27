Produced via MacWhisper from a recording of our Teams meeting

It's not perfect. My mic could have been better. But, as you will see, it was good enough

---

Speaker 1
Okay. Alright, so we're we're gonna brainstorm the uh new video approvals. um module feature thing. Right. Um and I'll I'll do like later on I'll do the sort of technical scene setting for it so knows sort of what language and framework and stuff to be doing it with. Really I just want you to to describe every everything you want it to do.

Speaker 2
Okay. Yep. All right. Can you help me out as well when I get stuck?

Speaker 1
Yeah, sure. I mean let's start with um What will they be using for?

Speaker 2
Okay. Okay, so basically uh for a very high-level overview, the approval system is a way of taking an object, whether it's a video or a photograph or a document and asking a number of people, one or more people, to review it and to comment on it. to see whether or not it is approved by them or whether it needs changes to be made. And if changes are made, then essentially you have a version of the original object. And that version then goes around and is recycled again for everyone to look at and comment on and approve or not approve. And that process carries on until everyone has approved this particular thing. So it's a kind of cyclical process um that ends when the object is fully approved by all members of the approval team.

Speaker 1
Okay. So let's let's let's do the scenario now where there is a video that needs to be approved. Uh sort of d drilling in inside the cycle. We're in that point now. We've got one video and uh a number of people need to look at it.

Speaker 2
Yeah, I mean I would say Jay, even before that, I think even before you've got the the object we we need to work out how the the the t the people work, the teams work, because obviously you need to associate that video with with with a with a team of of approvers. Does that make sense or would you rather just do the video? Yep, okay. So so I think I think really um uh in terms of approval by definition it kind of needs more than one person because if if there's only one person approving, they just they can just flick a switch to say this is approved. The whole point of the approvals system is that it's a collaborative workflow where you're interacting with more than one person or one with with a and at least one other person um and usually a team of people in order to uh to get their buy-in and their comments uh and eventually their approval on uh whatever the final version is. Therefore, I think the key thing here is to have kind of a a sort of roles uh roles and roles and permissions based sort of structure where at the very top you have the person who is the uh the manager if you like I can't think of a better word but the person who is who is organizing the approvals process for the the the object in question, let's say it's a video. Um they need to be uh or team needs to be created, an approvals team if you like, and as I say, that the manager sits sort of at the top of the team. Within the team you have approvers, i. e. people who have access to this video and have the ability to do whatever they need to do. So the approvers themselves, I would say There are probably a couple of levels of permissions, you know, ones who can see the video, ones who can um make make comments. Um uh and probably I can't think of anything else, but but let's just take it like that for for now.

Speaker 3
Okay.

Speaker 2
Um and the manager is the person who is going to be corraling these c these uh these comments together. So I think one of the important things is that uh when you've got a team who've got these permissions to to make comments, let's say, there needs to be some kind of alerting system. So for instance, I'm the manager and I put the video up I've created my team. I need to somehow alert my six approvers that this video has gone up and they need to take a look at it. You know, I I guess most obviously that would be via an email, but it could be via the app itself um you know they they they they're they're you know a bit like having uh uh alerts on any other app where you've got your little number of alerts in the on the dashboard or whatever it might be. But essentially, you know, the first thing is there is this video that's gone up. Please take a look at it. And then the six members can take a look. come into more detail in a minute about what they can do and what they can't do in terms of the video itself, which is what you're alluding to earlier. But I think that if they're making comments or drawing on the video or doing whatever else they're doing those comments then need to be um uh you know disseminated uh amongst the team and the team needs to be uh alerted to those. So again getting back to the roles and permissions probably what you need to be able to do is as a manager yes you receive everybody else's comments maybe there's permission where other the the other members of the team don't actually get pinged by the comments from other people. It's only the manager that that gets pinged, but they can see the other comments. So maybe there's a permission that that you're you can receive alerts from the other team or or you you you you you you can't depending on on uh on on the kind of team structure. I get it, yep. Um but but that that um you know that alert thing I think is kind of key to it really for the workflow. And really, you know, when s when something has been um you know commented on, obviously the the the the that the manager needs to know that the that person A has made a a a comment. Clearly if the manager then can respond to the comment to person A and say yes I agree or whatever. Um or that comment can can go out to the team. I suppose it's a bit like when you get an alert on uh Airbnb, you know, uh you get an alert saying, uh you ask the ask the post the question and they get back to you within the app. So Uh yeah. Uh whether or not that's done I think that's all done openly for for our intents and purposes, but but certainly the you know that kind of response Comment and response type thread is important. Now the the difficulty is obviously if you've got six people You don't want these comments to all be in one big stream of consciousness because otherwise it's going to look really co confusing. Or at least if it is in one long stream of consciousness, then um

Speaker 3
It's some somehow setting it out so that everybody's comments don't just get mangled up, you know, based on basically.

Speaker 1
I had an idea on that.

Speaker 3
Just just to drill in on that.

Speaker 1
That so we've got the the the lovely timeline metadata editor tool that we wrote for Ina.

Speaker 3
And I was thinking, well, what you could

Speaker 1
W that that would fit in their niceties, so each person gets their own row, as it were.

Speaker 3
Yeah, yeah, yeah. You could you could you know the the the supervisor can

Speaker 1
can sort of enable or disable different rows as they want and review each one independently.

Speaker 2
Yeah, I think that sounds that sounds good. Absolutely.

Speaker 1
Yeah, definitely.

Speaker 2
I mean in that case, what you could then do is then give the permissions on the rows so that person A can see rows, you know, C, D, and F, and you know what I mean, so that so that people can see whatever roles they're entitled uh rows they're entitled to see. Yeah, but I think that's not a bad idea.

Speaker 3
Yeah, yeah.

Speaker 2
That's a good idea, Jay. So I think um y y you know I I think key to this approvals thing as well is that uh uh you know you're you're kind of the the object the video let's say has a status, you know it's it's it's new, it's under review, it's been approved, and each person can set their own status. So each user can say I am reviewing or I have approved. Maybe three out of the six have approved, two are still reviewing. um one is kind of using the bit of some of the status you haven't started yet in the cycling. So again, so I think You know, that that's the the the the the general workflow and alerts and and you know making people aware of of you know the state the status has changed, this person's approved it and blah blah Um, yeah, it's it it is uh important. I think uh what else was I gonna say on that? Um the other thing is uh and I touched on it earlier is this concept of versions, you know. Let's say you've got all your feedback back and you know one person's approved but five who've got some some some changes they want to make. You want to be able to version the, let's say in this case, the video. So you've got version one um that has all the comments and then you're gonna upload a new version um for people to comment on and it's a question of keeping a nice tidy kind of filing system so that you've got the um you know the the the previous versions that you can go back to and look at in terms of uh you know whatever the comments were uh on the on the previous versions. So you know the the the manager or supervisor as you say would would be uh corraling all the comments got back that's fine they they go off and create a new video with some edits and stuff stick he sticks up the new version and the process begins uh again but uh as I say it's it's it's having a a container if you like for the the the the the the the the versions of the uh of the bit of content that's been reviewed.

Speaker 4
And does RTL kind of do some of that already? RTL, uh yeah, I mean it has a parent the concept of a parent child, but I think it's ugly in RTL.

Speaker 2
I think it would be much more like you know if you're uh if you're using Finder or something, you know, I think that kind of a uh a a more normalized UI where people are used to where they can drop something drop a file. And and create you know flexible or any number of hierarchies by by having those files in a kind of finder type structure, if you know what I mean. Right, right, right. Would be would be would be better. Because it doesn't need to be super sophisticated, it just needs to be tidy.

Speaker 1
Do you anticipate um reviewers could be reviewing um simultaneously?

Speaker 2
So Bob could be both be reviewing the same video at the same time. And that's very likely, yeah, absolutely. Okay.

Speaker 1
So we've got to be able to um Yeah, those things.

Speaker 2
Okay. Yeah, so I think as I say, it's the that that concept of the supervisor creating even before the video has even been looked at creating the team assigning roles and permissions to the team uh you know creating the the file structure where the video or the the picture lives um in the back end anyway at least and then dropping that bit of content into the app on the front end and that then alerting the team members, each of whom have different permissions to be able to comment or not comment or see other people or not see other people. And then maybe comments to interact, um, as you would interact on an app like uh you know like Teams or what it would be like Teams really. I mean it's it's pretty much the same kind of concept where you're just sort of pinging each other and having conversations. I mean Teens is actually quite a good example of how the comments might work within the uh you know within the app itself because you can see well the people on the left hand side of your project and um and when they're pinging you messages you can you know you can see them But those messages may also want to be sent uh via email and that might be a setting that you have when you're setting up the particular project. Please alert me by email, yes or no. um you know uh as well so because you may not want to have 5,000 emails um going backwards and forwards or you might want to um Okay.

Speaker 1
Um so so let's let's drill into the actual um guts of uh I'm a reviewer and the videos uh uh I've loaded up a screen. There's a as a as a s uh there's a screen with a video on it and what are the tools that I see, what can I do?

Speaker 3
Um

Speaker 2
I I think, you know, off the top of my head, and Jay, maybe you may have come across a few more in the course of what you've been doing, but I mean it's it's the kind of thing. It's the kind of ones that you would expect. I mean you've obviously got to be able to, on a video, be able to mark a timeline in and out where you want to make a change. So it's it's it's marking that timeline in and out. uh at a very basic level and putting a comment against it. But you know in a more sophisticated way you might want to mark the timeline in and out and draw something on the video or write on the video. Um I I I'm just trying to think, you know, beyond that, uh, I don't know, did you did you find anything did you do anything else in terms of the the the widgets that you had when you were looking at the that other bit of software?

Speaker 1
Oh no, so we had um obviously had the sort of the pencil drawing thing where you could just sketch with a variety of thicknesses and and line thicknesses and and a choice of colours. Then you could draw a box um with a with a border of whatever thickness.

Speaker 3
Okay.

Speaker 2
Could you could you have a text? Uh well we did text as a separate thing.

Speaker 1
It was just you can drop text in. Um but you could sort of merge the text feature into the box. So a box could optionally have text.

Speaker 3
That would be nice, yeah, absolutely. Okay.

Speaker 1
So okay, so you could put text inside the middle of a box and then And then the the filler of the box is, you know, is it is is it a border that's transparent uh inside or is it has it got a colour or is that or is it or is it a semi-transparent color?

Speaker 2
Um Yeah, I mean I I y that may be something that that is just a sort of uh an admin setting within the system rather than the user themselves being able to do, but it'd be nice to be able to to do that. The other thing it would be, you know, obviously it would be good to do is um bum bum bum bum bum maybe the uh users have that have a that can be assigned a colour, you know, uh in terms of the the the colour of the t the text when they're writing. You know, Bob's pink and and you know Jane is green or something. So that When you're looking at the screen, you kind of know who's made the comment just by looking at the the colour. Oh, yeah, good idea.

Speaker 1
Rather than them picking the colour of their things.

Speaker 2
Yeah.

Speaker 1
They're just what they're drawing is assigned their colour.

Speaker 2
Yeah, that's the sort of supervisor thing that they can define that absolutely. Maybe even define the font as well or the font side. But you know Um but I think those are the key things. You know, as long as that that's kind of captured the time with the timeline, I think that's uh really, really the main uh you know the main I've got I've got I've got I've got to tell it

Speaker 1
exactly what drawing tools we want. I've got to spell them out. So we've got obviously got drawing with a pencil.

Speaker 2
Yeah. Drawing an arrow. Just going to jump onto word onto Word and see. what we've got. Drawing with an arrow, absolutely. You've got obviously you've got your eraser.

Speaker 1
Yep.

Speaker 2
You've got your drawing fitness. You've got your um maybe your highlighting pen as well. Alright, I like it. Yeah. Uh do do do do and then what else have we got in on the insert? Yeah, icons. I mean I think it's good to insert some icons or some shapes. you know definitely arrows are good um and i suppose the cat the the library of shapes that you could insert um are you know I suppose that could always be that you know you you could have that as being some kind of um you know bolt-on thing where you can you know you can get more i more icons if if you want to. But I guess if you look at Word and look at the the typical shapes that you have on Word, they are arrows. They're arrows that have a little wiggly line where you can go from one point to another. um you know so you do the two points and then you join them up with an arrow that might be a bit of a bit of a curvy one. You've got your your sort of lines, straight lines or curvy lines and um yeah your basic shapes triangle circle square. uh uh you know what what have you. You might want to have a couple of stickers if you want like a smiley face or a love heart. Um but I think that you know uh Uh I think uh this it's generally those, but but lines, arrows, basic shapes, some sort of little approval thing like thumbs up or a smiley face or like don't like this, like a sort of sad face or

Speaker 1
a thumbs that you want to do. We've got in teams, like like we've got like if I if I just do that to your message, I can I can do that, I can love it, or I can Yeah, it's it's exactly right.

Speaker 2
So somebody makes a comment as well.

Speaker 1
So that

Speaker 2
That heart could be on the thumbs up, could be on the comment like in in teat.

Speaker 3
Yeah.

Speaker 2
Um so the you know the supervisors got back and done the thumbs up or whatever uh or you know just as a quick a quick acknowledgement or you know um they could do it within the com within the comment itself on the video if you know what i mean so with if someone some person takes the box the uh supervisor could put a little you know, a little thumbs up on the on the box as well. Right.

Speaker 1
Okay.

Speaker 2
But I think it's I think it's I think it's fairly it's doesn't have to be too many, you know, uh types of of of thing. But the the width Definitely. And the um, you know, uh highlighter would be good. Um and the actual uh um Yeah.

Speaker 1
Yeah. And um uh we talked about transformations before and we agreed that just zooming in and out was

Speaker 2
I think that's right. Yeah. We don't need flipping or uh yeah, absolutely. I think that's right.

Speaker 1
And so if you're zoomed in, you're sort of three hundred percent, you're just looking at sort of one upper corner of something. You should still be able to annotate on top of there, still be able to draw and everything, and then when you zoom back out, your drawing will have shrunk.

Speaker 3
Yeah, it shrunk. Yeah, accidentally.

Speaker 1
So you you can basically annotate

Speaker 2
At any zoom setting and it'll all just you might zoom out and then stick a great big arrow on across the screen pointing to the little thing in the corner say and you know and say zoom in on this

Speaker 1
Right, right. Right.

Speaker 5
Okay. Um, I'm trying to remember what else there was. I think that's it.

Speaker 2
other things. One thing I will say though, Jay, is is, and it's going back to the transformations, you don't really try to do transformations on video, however However, if you think about approving produx, let's say a teddy bear Um that teddy bear needs to be kind of rotated, you know, because it's the back of the teddy bear and the side of the teddy bear and the you know the front of the teddy bear. Now I don't know how you deal with that. Because you've got a 3D image effectively and whether that's a sort of file type.

Speaker 1
But yeah, that that isn't so what I was thinking is that the like the approvals um module, you know, it's got all of the um like the uh you know the person and and they can you know they there's a layer that they can sketch on but what they're sketching on Um you know we've talked about video, but that's just a layer. It could be that could be swapped out with a different type of layer, such as a 3D. There's a 3D module, 3JS, I think it's called. Right, right. For managing 3D objects that you can There's a WebGL one as well. I mean, whatever, it doesn't matter. And and the same thing would apply, for example, to a PDF. that you know it's it's it's just presented in a layer underneath that the the sort of transparent thing on top that you can sketch on it. You know the difference with the PDF is that obviously you can scroll it.

Speaker 3
Um so you know there's more than just what the the rectangle that's on the screen.

Speaker 1
Um it should be able to conform to any kind of thing underneath

Speaker 2
Exactly. I mean I think I think if you think of it in more sort of um let's let let's imagine that we're architects, right, and we've got um an image of someone's kitchen and we want to kind of like Turn the kitchen around, look at it from the ceiling point of view, look at it from a fleas point of view, looking up, different perspectives, you know, and therefore It's the same with approvals for a teddy bear or a football shirt or something. You've got to be able to s to to to w to look round it and upside down and underneath and you know what I mean? So so if there is software out there that does that uh and then you can have the layer on top of it. The only thing that I don't understand is if you're writing if you're making a comment on the front of the teddy bear Uh uh how does the how does the layer know that it's at the front? I suppose it it would do, right?

Speaker 1
Um Yeah, you'd have to you'd have to know you'd have to understand what kind of transformation is happening underneath and be associated with That specific transformation. So then when you review the comments as you step through them, um that transform that that comment can apply the transformation to it's exactly right, exactly right.

Speaker 2
It flips the image Because it's captured where the image was in terms of its transformative position. Yeah.

Speaker 1
Yeah.

Speaker 2
Uh yeah. And I don't know how but that that's sort of uh that that could uh I think I think that's I mean I don't think that's something that

Speaker 1
would do on MVP, but I think it's really worthwhile knowing that you want to do that. And so that you can write the uh the interface between those two layers, you can you can have a good abstraction Defined so that when you want to implement different types of layers underneath, um it's not gonna be a full Gory rewrite, it's gonna be uh we thought about that.

Speaker 2
And I think I think on that point, in in the sort of MVP in that case, you know, going back to the the original object or the the original file, whatever that is, whether it's a video file or an image, if you if you can't do a 3D thing, obviously something like a teddy bear, you'd have to have five photographs, right? Because you've got side, you know, up, down, whatever. So therefore, um what you're approving, it may be more than one file. You know, at the at the level, at the approval level, you're looking at five different files. They're not children, they're sick next. Or a drop-down person to select which one you want. Yeah, absol absolutely. Because uh because you know without a three D concept on on MVP you'd you kind of have to have that.

Speaker 1
Yeah.

Speaker 2
But I agree about the layer thing. I think uh in terms of the tools, it's really that basic stuff, the kind of stuff that you just get on on on Word really, you know, which is just variety of pencil uh wit widths um somebody being able to set a colour for each user, an eraser, and text boxes and different shapes of and some n you know a smattering of of of uh icons really for Yeah, like the ones that you've got there, you know, thumbs up and heart and happy face, sad face, um and uh and so forth.

Speaker 1
Got it. Okay. All right. I my call with the guys is at 9.

Speaker 2
30, so Okay, well I hope that's helpful. No, that's really useful.

Speaker 1
I mean I've got half an hour of text basically that that that brainstorms a thing.

Speaker 6
When you've sort of um got it put it through the through the AI, you know, whack it over and I'll take take a look.

Speaker 1
Oh thank you.

Speaker 3
Yeah, great.

Speaker 6
Alright, I'll do that. Um okay, cheese and j captionator, bye.

