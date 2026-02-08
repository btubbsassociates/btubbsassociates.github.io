---
layout: post
title: "Short interval control – the discipline of performance review"
date: 2023-03-01 10:00:00 -0800
categories: operations-management
author: Bill Tubbs
---

Short interval control (SIC) is an essential component of an operations management system and the foundation on which performance management is built. Yet, it is often neglected in this age of digitalization and big data.

![Formula 1 visor cam showing lap time display](/assets/images/blog/racing-visor-cam.png)
*Image source: FORMULA 1, Kimi Raikkonen Mode! (Visor Cam) \| F1 Testing 2019, YouTube.*

To understand the essence of SIC, consider a race-car driver who aims to complete a defined number of laps on a race track in the shortest possible time. I'm not an expert on motor racing, but I imagine there is a lot of advanced technology and real-time information provided to the driver. But what do you think is the most important metric of performance that a driver can use during a race? I'm curious to know what they would say, but I'm almost certain they would tell you it's their lap time. Without a measure of your lap time each time you complete one lap of the course, how can you know how well you are doing? How can you know whether the particular maneuver or technique you attempted in the last lap actually made a difference?

Short interval control in a process plant is the equivalent of using lap times during a race, or during training, to review and continuously improve performance. Obviously, in a chemical plant there are no lap times, so SIC is done on a time interval, typically every hour, by comparing cumulative actual production with cumulative planned production since the start of the current shift. This is done on a simple control sheet located on the desk in the control room, or electronically on a screen. At the end of each hour, the operator records actual production compared to target, and the reason for any deviation (i.e. losses) and what action was taken.

## Mental models

SIC is based on the principle that we use [mental models](https://en.wikipedia.org/wiki/Mental_model) to decide what action to take. In the classic book on systems thinking, *The Fifth Discipline*, Peter Senge described how humans construct mental models of reality, which he described as

> deeply ingrained assumptions, generalizations, or even pictures and images that influence how we understand the world and how we take action.

Mental models are particularly relevant when operating process plants because the process itself is not directly observable. Instead, the operator must infer the state of the process from the available measurements. To enable this, central control rooms in modern plants have arrays of monitor screens displaying thousands of process variables in real-time. These human-machine interfaces (HMIs) allow a few operators to monitor and make adjustments to large, complex facilities to ensure the process is operating safely, within operating limits, and to ensure it runs efficiently, or at maximum capacity. We rely on operators to process all that information—to decide what information to focus on, how to interpret it, and to make timely decisions on what interventions to make. But how good are our mental models? Who is checking the 'lap times'?

![Control room operator](/assets/images/services/process-control.jpg)
*Control room operator.*

If you ask a control room operator how they do their job, you will not get a simple answer. This reflects the complexity of modern process plants and the inherent difficulty of the job (if what they do could be defined, it could be done by a machine). But it's interesting to ask a different question, such as "what is total production so far today and are we on track to meet today's target?" The answer to this will provide clues as to whether they are using SIC. If they say they are not on track, ask them what the main cause (or causes) are. If they can answer that question without hesitation, and with facts, you know they are doing some form of short interval control.

I once asked an operator of a large offshore oil and gas platform these questions. He showed me the actual production rate which he was monitoring in real time on the HMI screen. When I asked about cumulative production so far today and whether they were on track to meet the daily production target, he responded with "that information is in the production report which the supervisor produces at the end of the day." In fact, he could not even calculate cumulative production even if he wanted to. Supervisory control and data acquisition (SCADA) systems are designed for real-time monitoring and control. They are not set up in a way that allows process performance to be monitored and managed.

## The automation paradox

It's important to acknowledge that safe operation is paramount. In that sense, the racing car analogy is not a good one—we don't want operators to run the plant so close to safe operating limits that there is a realistic chance they could be exceeded. And we don't want to distract operators from their primary task of continually checking key process variables. Their main job is to anticipate, or quickly detect, abnormal situations and take appropriate, timely action. Seeking to run the plant at its optimum operating point, is secondary, something they do at times when everything is running smoothly and there are no risks to safety or the environment.

Incidentally, the problem known as the [automation paradox](https://en.wikipedia.org/wiki/Automation#Paradox_of_automation), has led to the situation where operators today have less and less to do. As a result, management are now looking for ways to keep them engaged in the process so that they maintain good [situation awareness](https://en.wikipedia.org/wiki/Situation_awareness) in the event that they have to take over from the automation system. It can be argued that utilizing operators for performance management by implementing SIC is a solution to this problem—it forces the operator to keep their mental model of the current state of the process up to date.

![Diagram showing mental model, process KPI, and actions over time](/assets/images/blog/mental-model.png)
*Humans use mental models based on past experience to make predictions from recent observations.*

The main thing that SIC does is to enforce a feedback loop—it ensures operators repeatedly execute the plan-do-check-act routine at a regular interval. This is the key to learning. Not only are deviations detected in a timely manner and corrective action taken, the result of the action is evaluated with the facts, and the operator's mental model is thus updated.

Without SIC, it is unlikely that performance will continuously improve. By implementing SIC, you set the expectation that measuring, reviewing and reporting performance is a part of an operator's job. This then opens the door to coaching and training opportunities—it should not be a surprise when the shift supervisor comes over to discuss process performance with an operator. With SIC, the facts are clearly visible and "on the table."

## Towards a learning organization

Implementing SIC is the first step towards building a [learning organization](https://en.wikipedia.org/wiki/Learning_organization). While the central control room operator is primarily responsible for maintaining a safe and efficient operation, they are also in the best position to be the gatekeepers of performance for the whole organization. Although they are not fully responsible for plant performance, for example when there is an equipment breakdown, they have the facts and figures to quantify and record the loss and the circumstances under which it occurred. This kind of information is not recorded in process information systems and is almost impossible to dig up after-the-fact.

Most organizations have implemented some form of loss accounting—the practice of recording lost production and its causes. Lost production is defined as saleable output that could have been produced but was not for some reason. It is common to report plant availability (% of time running) or downtime, but these are not the whole story because they neglect the lost production due to lower-than-achievable production rates when running, which the control room operator is in a position to explain (hopefully).

In practice, production losses are usually calculated and reported by the production supervisor at the end of a shift or 24-hour period. While the supervisor has more experience and knowledge than a typical operator, they will not have the first-hand experience that an operator has of what was going on throughout the plant over the course of the shift. This is where a review of the completed SIC with the control room operator at the end of the shift is valuable. Not only is it a chance for the supervisor to question or challenge the information on performance, it shows operators that they have a direct and valuable role in performance management. It's not "something that the supervisor does at the end of the shift."

The benefits to operators are just the tip of the iceberg in terms of what SIC enables when integrated into an organization's loss accounting and performance management systems. In a future article I will introduce the concept of a choke model, which is used to decide where in the production process to install SIC.

## In summary

Why is SIC essential in any process plant operation?

1. Timely intervention to address performance problems
2. Triggers learning by challenging mental models
3. Accumulates the evidence needed by the organization to improve.
