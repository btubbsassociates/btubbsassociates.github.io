---
layout: post
title: "The choke model – start with the facts on losses"
date: 2023-03-19 12:13:00 -0700
last_modified_at: 2023-04-23 12:13:00 -0700
categories: operations-management
author: Bill Tubbs
---

A choke model analysis is the starting point to understanding production losses, where they originate in the process, and what is causing them.

![Image of pipework in a process plant or refinery](/assets/images/blog/process-plant-pipework.jpg)
*A complex process plant*

In the [previous article](/post/article-short-interval-control), I described short interval control (SIC)—the discipline of reviewing process performance during a shift and collecting information on losses. But in a complex production plant with multiple, interconnected units, where should losses be recorded? In this article, I define production losses and introduce the concept of *choke points* and the *choke model*, used to identify where to install SIC and where to focus improvement efforts.

Lost production is defined as saleable output that could have been produced but was not, for some reason. Obviously, this definition encompasses a vast array of possible causes. Rather than attempt to record and act on every possible event or cause, [*loss accounting*](/post/article-loss-accounting) is a process of quantifying and capturing lost production by assigning it to categories that can later be aggregated and effectively analyzed, so that problem-solving efforts can target the biggest and best opportunities.

*Choke points* are steps in the value chain where throughput is often less than the capacity of the equipment. It's important to understand the difference between a choke point and a *bottleneck*. Most process engineers are familiar with the concept of a bottleneck, which is a physical constraint that occurs at the point in the process where the equipment with the lowest capacity is installed. The bottleneck determines the overall maximum possible sustainable throughput of the whole plant—that's why process engineers look for ways to remove it. However, process units do not operate at full capacity all the time, so the bottleneck does not explain actual production and is therefore of little use in reducing losses.

Unlike bottlenecks, there may be, and usually are, more than one choke point where losses occur, including but not limited to the bottleneck. To get started with optimizing production, a choke model is needed. A choke model is a diagram of the main choke points in the process and the quantified actual losses at each, usually based on a recent 12-month period of operation. Figure 1 below shows choke points in two process examples. The first is a mining process which is linear. The second is a process called *steam-assisted gravity drainage* (SAGD), used in unconventional oil production, which has a water recycle stream. Note that both processes have multiple potential choke points.

![Two examples of production processes each with choke points.](/assets/images/blog/choke-point-examples.png)
*Figure 1. Examples of choke points in two production processes.*

A choke model is an analysis of the actual losses that occur at each choke point. To do this, the actual throughput at each choke is analyzed using historic data (usually hourly production data) over a period of 3-12 months, and compared to the maximum achievable hourly rate. Anything below the achievable rate is a loss. These are then reviewed with key people (operations, maintenance, planners, etc.) to determine the causes. Production logs and maintenance records may also be used to shed light on what was behind certain events. The reasons are then grouped into logical categories. It's important not to leave out any losses. If necessary, a bucket for "unknown" losses should be used.

If insufficient data is available to retroactively determine all the causes of lost production, then it may make sense to implement SIC on a temporary basis at one or more choke points to determine what is actually causing the losses. Although losses over a short period will not reflect typical losses over a year, they will help quantify the small, persistent, re-occurring losses, which are often less well understood.

Every plant is unique, so the location and significance of choke points will vary. In one operation, the mine might be the biggest cause of lost final production. In another, it might be the grinding process. In some operations, equipment reliability is the biggest cause of lost production, in others, it is rate losses due to variability or disturbances. It depends on many factors, such as the complexity of the process, the capacity of the equipment, its age, reliability, and how it is operated.

As illustrated in Figure 2 below, a good choke model quantifies the losses at each choke point and provides a breakdown of the main causes. In most operations, discretionary time and resources are in short supply, yet there are many possible improvement projects to work on. Based on the choke model, the organization can design a systematic improvement program to gain maximum benefits by focussing on the biggest losses or loss categories currently impacting production.

![Choke model diagram showing losses at each choke point.](/assets/images/blog/choke-model.png)
*Figure 2. Example of a choke model*

However, the biggest opportunities are not necessarily those associated with the biggest losses. The 'impactability' of losses must also be taken into account. If, for example, considerable effort has already been made to reduce the duration of the annual shutdown, then it may be that further reductions in this loss category are not possible. On the other hand, focussing effort on something that does not cause a significant proportion of the annual loss, will never yield substantial benefits. Sometimes common themes emerge when analyzing numerous loss events. For example, common failure modes such as pump impeller failures, or pipe joint leaks, or operator error. These point to opportunities that could be addressed by a targeted program.

A choke model also provides insights on where SIC and loss capture should be implemented. In the example in Figure 2, it might make sense to install an SIC on the mine production and also on the grinding process. However, there are other things to consider when deciding where to install SIC, such as available and accurate metering, boundaries of organizational responsibility, and the location of storage facilities (i.e. tanks or stockpiles), which effectively isolate one process step from another.

## Theory of constraints and line balancing

Choke models are closely related to the [*theory of constraints*](https://www.leanproduction.com/theory-of-constraints/) which is a methodology to identify the limiting factor in a process and then systematically improve it until it is no longer the constraint. In lean manufacturing doctrine, the technique of *line balancing* is used to synchronize and subordinate all steps in the production process to the rate at the current constraint. This makes it immediately apparent which step in the process is causing a line slowdown or stoppage.

Line balancing is difficult to achieve in large process plants, which have complex dynamics, and where temporary adjustments to production rates are avoided whenever possible. For these reasons, process plants tend to rely on intermediate product storage to absorb temporary imbalances. Any imbalance in inventories remaining at the end of a day is then corrected by the supply and operational planning process (S&OP) which determines the optimal production plan for the next day. Although not as conceptually simple as line balancing, this achieves the same goal of subordinating overall production to the actual constraints.

Ideally, we would like to attribute losses in final production to losses at specific choke points. However, this can be difficult to do in the absence of line balancing. Typically, in a linear process such as the first one in Figure 1, chokes that are downstream of the most significant choke point will frequently report losses due to a lack of feedstock. Likewise, chokes upstream of a significant choke will report downtime due to downstream rate reductions or lack of downstream storage. In this case, it is not too difficult to see where the problem is.

In the case of a circular production process such as in the SAGD example in Figure 1, the processes at each choke point might be frequently shutting down or reducing rate due to lack of supply or downstream capacity—i.e. shortage/excess of steam for well production, shortage/excess of produced water for water treatment, and shortage/excess of boiler feed-water for steam production. In this case, it is unclear which choke (if any) is the problem. It might point instead to a serious production planning and scheduling problem, or a lack of intermediate storage capacity. It is not uncommon for operations to be stuck in a kind of trap—the S&OP process doesn't function because production is too erratic to predict, or it is not based on actual production performance. At the same time, achieving consistently high production in individual processing units is difficult because of constant supply/demand interruptions.

The advantage of the choke model approach is that you don't need to resolve the S&OP problem to start tracking [*overall equipment effectiveness*](https://en.wikipedia.org/wiki/Overall_equipment_effectiveness) (OEE) and acting on losses at the critical choke points. The goal is to identify the key choke points and use the facts on losses to drive initiatives that increase OEE at those points. Whether production is lost due to a breakdown or a scheduling problem, it is a lost opportunity to utilize valuable capital equipment and should be recorded. Once equipment availability and throughput are consistently at high levels, and these have been quantified, it is easier to solve the S&OP problem.

Over time, the losses at each choke point will change. As losses are permanently eliminated at one choke point, they may increase at another. Therefore, the choke model will evolve and need updating over time. The focus of SIC and improvement efforts should also shift accordingly.

In the [next article](/post/article-loss-accounting), I describe the loss accounting process in more detail and how to use it to drive continuous improvement. Once a loss accounting system is in place, production losses are tracked and reviewed as a matter of course, and used to guide management decision-making and set improvement priorities.

## In summary

What are the benefits of a choke model?

1. Identifies the points in the process where production losses occur
2. Quantifies the historic losses and identifies the main causes
3. Indicates where SIC and loss accounting should be installed
4. Consensus on where to focus improvement efforts.
