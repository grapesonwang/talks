---
layout: slides
title: Natural and Artificial Intelligence
author: Neil D. Lawrence
institute: Amazon Research Cambridge and University of Sheffield
bibliography: ai-revolution.bib
---
<!--notes:
- a plastic plant. is poor. It is poorly define
- it may with us for the did not join us It’s intelligence is based The worth of an idea  A negotiated compromise betwagreed upon , because it is predicated on a shared condition. The constraints on . A shared limitations.  is this condition. This locked in intelligence, because however we create an artificial intelligence it will 
- The challenge for an artificial intelligence is to emulat
-, an ingrained world view.or is predisposed to certain
- to seek out teleological explanations. 
- Each of To have a shared understanding on intent, we need a shared understanding of each other, of how we’ll likely react to different circumstances. We do this through empathy, through our artificial systems are able to communicate any of their thoughts far While communication does not have to be part of an individuals intelligence, if we consider the populations intelligence, we see that the architecture for sharing information wilI if we assume that sharing of information between individual computers or humans is a key 
- The average word in English contains 12 
- The challenges of this new form of systems design have already been explored in systems biology, a field dedicated to the reverse engineering of biological systems. As many researchers have found, classical approaches to reverse engineering, which typically involve subjecting the system to a perturbation. In other words actively changing the system, to obtain a deeper understanding of behaviour normally fail because a natural system will often compensate. Survival dictates that there should be back up systems that kick in. 
- Robust approaches to systems design for the “don’t fail” predicate are beyond the scope of current engineering practice. They require uncertainty, best default behaviours, worst case analyses. They require you to consider how your artificial intelligence should respond to a mischievous 10 year old. 
-  (in the simplest case, hitting it with a hammer
- Firstly, imagine all the different pin configurations there could be in our hyperspace pinball machine. There are many pin configurations that may work well, but in such a complex machine, even if we have a lot of data to test it with, there may be areas of the machine we don’t explore until we test it in the real world, unforeseen circumstances. How do we guarantee that the machine doesn’t mess up?
- Or what if we get the objective function wrong? How do we distil our desired behaviour into a simple mathematical function. 
- *Pigeonholed activity*
- *Natural vs artificial systems*
- *natural vs human intelligence*
- The prediction function is the object that is used to make new pr
- that we are a long way off. Or at least, there are technological breakthroughs that need to happen 
So what will be the last bastion 
- In the timeliSuper human performance on specific tasks are hailed as breaDebates around artificial intelligence are confused because the fail to properly define tBroadly My own position is Human intelligence is quite diffrArtificial intelligence is a loaded term, one that is challenging because it means different things to different people. Historically, artificial intelligence practitioners focussed on planning and logic. Recreating the reasoning abilities of humans in our artificial devices, but the new wave of breakthroughs come from something else. From artificial neural network models. 
- However, just as the origins of Although the origins of - One challenge is that most practitioners of artificial intelligence do not give 
- Or at least in emulating a set of actions that we regard as intelligent. Whether it’s 
-->
\ifdef{ipynb}
\define{\includesvg{filename}}{<img src="\filename">}

\else
\define{\includesvg{filename}}{<object class="svgplot" data="\filename"></object>}
\endif
\define{\includeimg{filename}{width}{class}}{<img class="\class" src="\filename" width="\width" style="background:none; border:none; box-shadow:none;">}

*How are we making computers do the things we used to associated only with humans? Have we made a breakthrough in understanding human intelligence?*

While recent achievements might give the sense that the answer is yes, the short answer is that we are nowhere near. All we’ve achieved for the moment is a breakthrough in *emulating intelligence*. 

\includeimg{../slides/diagrams/science-holborn-viaduct.jpg}{30%}

<center><i>Science on Holborn Viaduct, cradling Watt's Governor</i></center>

Artificial intelligence is a badly defined term. Successful deployments of intelligent systems are common, but normally they are redefined to be non-intelligent. My favourite example is [Watt’s governor](https://en.wikipedia.org/wiki/Centrifugal_governor). Immortalised in the arms of the statue of “Science” on the Holborn viaduct in London, Watt’s governor automatically regulated the speed of a steam engine, closing the inlet valve progressively as the engine ran faster. It did the job that an intelligent operator used to have to do, but few today would describe it as “artificial intelligence”.

A more recent example comes from the middle of the last century. A hundred years ago *computers* were human beings, often female, who conducted repetitive mathematical tasks for the creation of mathematical tables such as logarithms. Our modern digital computers were originally called *automatic computers* to reflect the fact that the intelligence of these human operators had been automated. But despite the efficiency with which they perform these tasks, very few think of their mobile phones or computers as intelligent.

## Cybernetics

* Norbert Wiener launched last century’s first wave of interest in emulation of intelligence with his book “Cybernetics”. The great modern success that stemmed from that work is the modern engineering discipline of Automatic Control. The technology that allows fighter jets to fly. These ideas came out of the Second World War, when researchers explored the use of radar (automated sensing) and automatic computation for decryption of military codes (automated decision making). Post war a body of researchers, including Alan Turing, were seeing the potential for electronic emulation of what had up until then been the preserve of an animallian nervous system. 

So what of the modern revolution? Is this any different? Are we finally encroaching on the quintessential nature of human intelligence? Or is there a last bastion of our minds that remains out of reach from this latest technical wave? 

## Two Answers

1. Current technology is a long way from emulating all aspects of human intelligence: there are a number of technological breakthroughs that remain before we crack the fundamental nature of human intelligence.

2. More controversially, I believe that there are aspects of human intelligence that we will never be able to emulate, a preserve that remains uniquely ours. 

## Review of Current Technology
 
* Recent breakthroughs in artificial intelligence are being driven by advances in machine learning. Or more precisely, a sub domain of that field known as deep learning. So what is deep learning? Well, machine learning algorithms proceed in the following way. They observe data, often from humans, and they attempt to emulate that data creation process with a mathematical function. Let’s explain that in a different way. Whichever activities we are interested in emulating, we acquire data about them. Data is simply a set of numbers representing the activity. It might include location, or number representing past behaviour. Once we have the behaviour represented in a set of numbers, then we can emulate it mathematically. 

* Different mathematical functions have different characteristics, in trigonometry we learnt about sine and cosine functions. Those are functions that have a period. They repeat over time. They are useful for emulating behaviour that repeats itself, perhaps behaviour that reflects day/night cycles. But these functions on their own are too simple to emulate human behaviour in all its richness. So how do we make things more complex? In practice we can add functions together, scale them up and scale them down. All these things are done. Deep learning refers to the practice of creating a new function by feeding one function in to another. So we create the output of a function, feed it in to a new function, and take the output of that as our answer. In maths this is known as *composition* of functions. The advantage is that we can generate much more complex functions from simpler functions. The resulting functions allow us to take an *image* as an input and produce an output that includes numbers representing what the objects or people are in that image. Doing this accurately is achieved through composition of mathematical functions, otherwise known as deep learning. 

## Pinball Analogy

* To describe this process, I sometimes use the following analogy. Think of a pinball machine with rows of pins. A plunger is used to fire a ball into the top of the machine. Think of each row of pins as a function. The input to the function is the position of the ball along the left to right axis of the machine at the top. The output of the function is the position of the ball as it leaves each row of pins. Composition of functions is simply feeding the output of one row of pins into the next. If we do this multiple times, then although the machine has multiple functions in it, by feeding one function into another, then the entire machine is in itself representing a single function. Just a more complex function than that that any individual row of pins can represent. Our modern machine learning systems are just like this machine. Except they take very high dimensional inputs. The pinball is only represented by its left to right position, a one dimensional function. A real learning machine will often represent multiple dimensions, like playing pinball in a hyperspace.

## Intelligence Emulation

* So the intelligence we’ve created is just a (complex) mathematical function. But how do we make this function match what humans do?  We use more maths. In fact we use another mathematical function. To avoid confusion let’s call the function represented by our pinball machine the *prediction function*. In the pinball machine, we can move the pins around, and any configuration of pins leads to a different answer for our functions. So how do we find the correct configuration? For that we use a separate function known as the *objective function*. 

* The objective function measures the dissimilarity between the output of our prediction function, and data we have from the humans. The process of learning in these machines is the process of moving the pins around in the pinball machine to make the prediction more similar to the data. The quality of any given pin configuration is assessed by quantifying the differences between what the humans have done, and what the machine is predicting using the objective function. Different objective functions are used for different tasks, but objective functions are typically much simpler than prediction functions.

## Algorithm Design

* So, we have some background. And some understanding of the challenges for the designer of machine learning algorithms. You need data, you need a prediction function, and you need an objective function. Choice of prediction function and objective function are in the hands of the algorithm designer. Deep learning is a way of making very complex, and flexible, classes of prediction functions that deal well with the type of data we get from speech, written language and images. 

## Brittleness of Current AI

* But what if the designer gets the choice of prediction function wrong? Or the choice of the objective function wrong? Or what if they choose the right class of prediction function (such as a convolutional neural network, used for classifying images) but get the location of all those pins in the machine wrong?

* This is a major challenge for our current generation of AI solutions. They are fragile. They are sensitive to incorrect choices and when they fail, they fail catastrophically.

## Artificial vs Natural Systems

* Consider natural intelligence, or natural *systems*

* Contrast between an artificial *system* and an natural system.

* The key difference between the two is that artificial systems are *designed* whereas natural systems are *evolved*.

## Engineering Systems Design

* Major component of all Engineering disciplines.

* Details differ: there is a common theme: achieve your objective with the minimal use of resources to do the job.

* This provides efficiency.

* Engineering designer imagines a solution that requires the minimal set of components to achieve the result.

* A water pump has one route through the pump.

* That minimises the number of components needed. Redundancy is introduced only in safety critical systems, such as aircraft control systems. Students of biology, however, will be aware that in nature system-redundancy is everywhere. Redundancy leads to robustness. For an organism to survive in an evolving environment it must first be robust, then it can consider how to be efficient. Indeed, organisms that evolve to be too efficient at a particular task, like those that occupy a niche environment, are particularly vulnerable to extinction.

* So it is with natural vs artificial intelligences. Any natural intelligence that was not robust to changes in its external environment would not survive, and therefore not reproduce. In contrast the artificial intelligences we produce are designed to be efficient at one specific task: control, computation, playing chess. They are *fragile*.

## Don't Fail

* First criterion of a natural intelligence is *don’t fail*.

* In contrast, mantra for artificial systems is to be more efficient.

* Artificial systems are given a single objective (in machine learning it is encoded in a mathematical function)

* Aim to achieve that objective efficiently.

## Designing out Failure

* Even if we wanted to incorporate *don’t fail* in some form, it is difficult to design for.

* To design for “don’t fail”, you have to consider every which way in which things can go wrong, if you miss one you fail. These cases are sometimes called corner cases.

* In an uncontrolled environment, almost everything is a corner.

    * It is difficult to imagine everything that can happen.
    
    * Most of our automated systems operate in controlled environments (e.g.  a factory, a set of rails.)

## Deployment in Uncontrolled Environments

* Requires a different approach to systems design.

    * One that accounts for uncertainty in the environment
    * One that is robust to unforeseen circumstances. 

## Pigeonholing

\includeimg{../slides/diagrams/TooManyPigeons.jpg}{60%}

## Robust

* Need to move beyond pigeonholing tasks.

* Need new approaches to both the design of the individual components, and the combination of components within our AI systems.

* Need to deal with uncertainty and increase robustness.

* Today, it is easy to make a fool of an artificial intelligent agent, technology needs to address the challenge of the uncertain environment to achieve robust intelligences.

## Embodiment Factors

* However, even if we find technological solutions for these challenges, it may be that the essence of human intelligence remains out of reach. It may be that the most quintessential element of our intelligence is defined by limitations. Limitations that computers have never experienced.

* That characteristic is our limited ability to communicate, in particular our limited ability to communicate versus our ability to compute. Not compute in terms of working out arithmetic or solving sudoku problems, but the amount of compute that underpins our higher thoughts. The computation that our neurons are doing. 

* It is estimated that to simulate the human mind it would require a supercomputer operating as fast as the world’s fastest. The UK Met Office’s computer, that is used for simulating weather and climate across the world, might do it. At the time of writing its the 11th fastest computer in the world. Much faster than a typical desktop. But while a typical computer seems to be performing less operations than our brain does. A typical computer can communicate much faster than we can. 

* Claude Shannon developed the idea of information theory: the mathematics of information. He defined the amount of information we gain when we learn the result of a coin toss as a “bit” of information. A typical computer can communicate with another computer with a billion bits of information per second. Equivalent to a billion coin tosses per second. So how does this compare to us? Well, we can also estimate the amount of information in the English language. Shannon estimated that the average English word contains around 12 bits of information, twelve coin tosses, this means our verbal communication rates are only around the order of tens to hundreds of bits per second. Computers communicate tens of millions of times faster than us, in relative terms we are constrained to a bit of pocket money, while computers are corporate billionaires.

* Our intelligence is not an island, it interacts, it infers the goals or intent of others, it predicts our own actions and how we will respond to others. We are social animals, and together we form a communal intelligence that characterises our species. For intelligence to be communal, our ideas to be shared somehow. We need to overcome this bandwidth limitation. The ability to share and collaborate, despite such constrained ability to communicate, characterises us. We must intellectually commune with one another. We cannot communicate all of what we saw, or the details of how we are about to react. Instead, we need a shared understanding. One that allows us to infer each other’s intent through context and a common sense of humanity. This characteristic is so strong that we anthropomorphise any object with which we interact. We apply moods to our cars, our cats, our environment. We seed the weather, volcanoes, trees with intent. Our desire to communicate renders us intellectually animist.
	
* But our limited bandwidth doesn’t constrain us in our imaginations. Our consciousness, our sense of self, allows us to play out different scenarios. To internally observe how our self interacts with others. To learn from an internal simulation of the wider world. Empathy allows us to understand others’ likely responses without having the full detail of their mental state. We can infer their perspective. Self-awareness also allows us to understand our own likely future responses, to look forward in time, play out a scenario. Our brains contain a sense of self and a sense of others. Because our communication cannot be complete it is both contextual and cultural. When driving a car in the UK a flash of the lights at a junction concedes the right of way and invites another road user to proceed, whereas in Italy, the same flash asserts the right of way and warns another road user to remain.

## Social Intelligence

* Our main intelligence is our social intelligence, intelligence that is dedicated to overcoming our bandwidth limitation. We are individually complex, but as a society we rely on shared behaviours and oversimplification of our selves to remain coherent. 

* This nugget of our intelligence seems impossible for a computer to recreate directly, because it is a consequence of our evolutionary history. The computer, on the other hand, was born into a world of data, of high bandwidth communication. It was not there through the genesis of our minds and the cognitive compromises we made are lost to time. To be a truly human intelligence you need to have shared that journey with us. 

## Emulation

* Of course, none of this prevents us emulating those aspects of human intelligence that we observe in humans. We can form those emulations based on data. But even if an artificial intelligence can emulate humans to a high degree of accuracy it is a different type of intelligence. It is not constrained in the way human intelligence is. You may ask does it matter? Well, it is certainly important to us in many domains that there’s a human pulling the strings. Even in pure commerce it matters: the narrative story behind a product is often as important as the product itself. Handmade goods attract a price premium over factory made. Or alternatively in entertainment: people pay more to go to a live concert than for streaming music over the internet. People will also pay more to go to see a play in the theatre rather than a movie in the cinema. 

## Artificial Plants

* In many respects I object to the use of the term Artificial Intelligence. It is poorly defined and means different things to different people.  But there is one way in which the term is very accurate. The term artificial is appropriate  in the same way we can describe a plastic plant as an artificial plant. It is often difficult to pick out from afar whether a plant is artificial or not. A plastic plant can fulfil many of the functions of a natural plant, and plastic plants are more convenient. But they can never replace natural plants.

## Conclusion

* In the same way, our natural intelligence is an evolved thing of beauty, a consequence of our limitations. Limitations which don’t apply to artificial intelligences and can only be emulated through artificial means. Our natural intelligence, just like our natural landscapes, should be treasured and can never be fully replaced. 

\include{../_ai/includes/the-diving-bell-butterfly.md}
\include{../_ai/includes/jean-dominique-bauby.md}
\include{../_ai/includes/embodiment-factors-tedx.md}

