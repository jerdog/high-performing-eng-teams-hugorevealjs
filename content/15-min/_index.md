+++
title = "High-performing Engineering Teams, and the Holy Grail"
outputs = ["Reveal"]
[reveal_hugo]
custom_css = "css/custom.css"
+++

### High-performing Engineering Teams, and the Holy Grail
![holy grail pfffft](/images/slides/anim-titleSlide-pfft.gif)

---

![dev productivity](/images/slides/devProductivity.png)
{.r-stretch}

{{% note %}}
Software delivery has never been more critical to the success of business in every industry. It’s also never been more complex. Expectations for delivering high-quality software incredibly fast have skyrocketed - yesterday’s most exceptional product experiences are expected today to be more beautiful, intuitive, powerful, and affordable.
{{% /note %}}

---

![cncf-landscape](/images/slides/cncf-landscape.png)
{.r-stretch}

{{% note %}}
But the landscape of tools, platforms, and architectures is constantly evolving. With this rapid pace of change and the growing challenges of complexity, how can engineering teams not only succeed but beat out the competition?
{{% /note %}}

---

{{< slide id="bio" transition="zoom" transition-speed="fast" >}}
<section>
    <div class="multiCol">
        <div class="col">
            <h4 style="color: rgb(111, 168, 220);">Jeremy Meiss</h4>
            <p style="font-size: .75em;">Director, DevRel &</p>
            <p style="font-size: .75em;">CircleCI</p>
        </div>
        <div class="col"><img src="/images/profile-pic.jpg" width="60%"></div>
    </div>
</section>

---

#### So back to the tech industry...

![Back to the Tech Industry](/images/slides/back-to-the-tech-industry.gif)

{{% note %}}
We have entered into a period of immense change, and with the global economic uncertainties presented impacting companies of all sizes.
{{% /note %}}

---

![You Seek the Holy Grail](/images/slides/you-seek-holy-grail.gif)
{.r-stretch}

{{% note %}}
Amidst this environment, stability and reliability have become increasingly important to businesses globally. The ability to provide a reliable, stable platform to customers has become a crucial value metric to engineering teams and will only continue to increase in importance this year.
{{% /note %}}

---

![state-of-reports](/images/slides/state-of-reports.png)
{.r-stretch}

{{% note %}}
Since 2019, we have been analysing the anonymous data from all of the jobs and workflows run on our platform, and we've identified a set of recommended baseline engineering metrics as related to CI/CD, and we've been able to paint a picture of what it means to have an elite and holistic software delivery practice. 
{{% /note %}}

---

![one size doesn't fit all](/images/slides/not-one-size.jpg "Image: Consumer Choice Center")
{.r-stretch}

{{% note %}}
We don’t believe in one-size-fits-all success metrics for delivery; because every team is different. However, the software delivery patterns we’ve observed, especially the data points from top delivery teams, show key similarities that suggest valuable benchmarks for teams to use as goals. 
{{% /note %}}

---

<section>
<h4>CI/CD Benchmarks for high-performing teams</h4>
    <div class="multiCol r-stretch">
        <div class="col">
            <img src="/images/slides/duration.png" height="60px">
            <p style="font-size: .5em;">Duration</p>
        </div>
        <div class="col">
            <img src="/images/slides/mttr.png" height="60px">
            <p style="font-size: .5em;">Mean time to resolve</p>
        </div>
        <div class="col">
            <img src="/images/slides/success-rate.png" height="60px">
            <p style="font-size: .5em;">Success rate</p>
        </div>
        <div class="col">
            <img src="/images/slides/throughput.png" height="60px">
            <p style="font-size: .5em;">Throughput</p>
        </div>
    </div>
</section>

{{% note %}}
This report covers the standard engineering metrics of Duration, Mean time to recovery, Success Rate, and Throughput, plus our recommended benchmarks for each. But the sections have been expanded to show how your team can optimize your practice through team structure, culture, and operational strategy, to ensure you’re maintaining a key ingredient in achieving success: developer happiness.  
{{% /note %}}

---

![dude this is a Wendy's](/images/slides/pipelines.gif)
{.r-stretch}

{{% note %}}
As CI adoption expanded over the last several years, many teams have had a “growth at all costs” mentality. But as the complexity of software systems increased, the cognitive load of maintaining those systems has really become overwhelming for both the devs and ops sides, creating situations where teams were cutting corners. DevOps teams must take away some of the complexity and be in a position to help systems recover quickly from failures. This is why many companies have instituted a Platform team — the need for a dedicated team to support the stability of their application has become obvious.
{{% /note %}}

---

![head banging good time](/images/slides/head-banging.gif)
{.r-stretch}

{{% note %}}
So you probably came to your talk with this question: "How do you achieve elite status through a holistic software delivery practice?" Or it was for the Holy Grail references. Either way, it's a good question. Let's jump into the data
{{% /note %}}

---

### Duration

_the foundation of software engineering velocity, measures the average time in minutes required to move a unit of work through your pipeline_

{{% note %}}
Duration is the foundation of software engineering velocity. It measures the average time in minutes required to move a unit of work through your pipeline. Importantly, a unit of work does not always mean deploying to production – it may be as simple as running a few unit tests on a development branch. It can be best viewed as a proxy for how efficiently your pipelines deliver feedback on the health and quality of your code. 
{{% /note %}}

---

![efficency](/images/slides/efficiency.gif)
{.r-stretch}

{{% note %}}
Duration, then, is best viewed as a proxy for how efficiently your pipelines deliver feedback on the health and quality of your code. The core promise of most software delivery paradigms, from Agile to DevOps, is speed: the ability to take in information from customers or stakeholders and respond quickly and effectively. 
{{% /note %}}

---

![rejoice rejoice](/images/slides/rejoicing.gif)
{.r-stretch}

{{% note %}}
These rapid feedback and delivery cycles don’t just benefit an organization’s end users; they are crucial to keeping developers happy, engaged, and in an uninterrupted state of flow. 
So what's the ideal duration?
{{% /note %}}

---

#### Duration Benchmark
##### <=10 minute builds

*"a good rule of thumb is to keep your builds to no more than ten minutes. Many developers who use CI follow the practice of not moving on to the next task until their most recent checkin integrates successfully. Therefore, builds taking longer than ten minutes can interrupt their flow."*  
-- **Paul M. Duvall (2007).**  *Continuous Integration: Improving Software Quality and Reducing Risk*

{{% note %}}
To get the maximum benefit from your workflows, we recommend aiming for a duration of 10 minutes, which is a widely accepted benchmark that dates back to Paul M. Duvall’s influential book on Continuous Integration. At this range, it is possible to generate enough information to feel confident in your code without introducing unnecessary friction in the software delivery process.
{{% /note %}}

---

#### Duration: What the data shows

![duration](/images/slides/duration-data.png)
{.r-stretch}

###### Benchmark: 5-10mins


{{% note %}}
Among the workflows observed in our dataset, 50 % completed in 3.3 minutes or less, far below our 10 minute benchmark and nearly 30 seconds faster than previous reports. The fastest 25% of workflows completed in under a minute, and 75% completed in under 9. The avg duration was approx 11 minutes, reflecting the influence of longer-running workflows in the 95th percentile require 27 minutes or more to complete.
{{% /note %}}

---

#### Improving test coverage

* Add unit, integration, UI, and end-to-end testing across all app layers
* Incorporate code coverage tools into pipelines to identify inadequate testing
* Include static and dynamic security scans to catch vulnerabilities
* Incorporate TDD practices by writing tests during design phase

{{% note %}}
Many teams continue to bias toward speed rather than robust testing. But, as shown here, the number one opportunity we’ve identified for improving performance across all four software delivery metrics is for organizations to enhance their test suites with more robust test coverage.
{{% /note %}}

---

![dancing efficiency](/images/slides/dancing-efficiency.gif)
{.r-stretch}

{{% note %}}
The path to optimizing your workflow durations is to combine comprehensive testing practices with efficient workflow orchestration. Teams that focus solely on speed not only spend more time rolling back broken updates and debugging in production but also face greater risk to their organizational reputation and stability.
{{% /note %}}

---

### Mean time to Recovery

_the average time required to go from a failed build signal to a successful pipeline run_

{{% note %}}
MTTR. This metric is indicative of your team’s resilience and ability to respond quickly and effectively to feedback from your CI system. In other words, mean time to recovery is the best indicator of your organization’s DevOps maturity.
{{% /note %}}

---

![pipeline time to recovery](/images/slides/time-to-recovery.gif)
{.r-stretch}

{{% note %}}
From an end user perspective, and for most organizations, nothing is more important than your team’s ability to recover from a broken build. While customers may not notice the steady stream of granular updates that you ship throughout the week, they will definitely notice when your application goes offline after broken code slips through your test suite.
{{% /note %}}

---

*"A key part of doing a continuous build is that if the mainline build fails, it needs to be fixed right away. The whole point of working with CI is that you're always developing on a known stable base."*  

-- **Martin Fowler (2006).** *"Continuous Integration."* Web blog post. MartinFowler.com

{{% note %}}
In a 2006 blog post, Martin Fowler described the north star for software teams’ MTTR: “Fix broken builds immediately.” Does this mean your team should aim for resolving failed workflows within a matter of seconds? Or better yet avoid build failures at all costs? Not at all! Broken builds happen, and with proper tests in place, the information from a red build has as much (if not more) value for development teams as a passing green build.
{{% /note %}}

---

#### MTTR Benchmark

###### <=60min MTTR on default branches

{{% note %}}
For this reason, we recommend that you aim to fix broken builds on any branch in under 60 minutes. Depending on the scale of your user base and criticality of your application, your target recovery time may be significantly lower or higher. However, the ability to recover in under an hour is strongly correlated with other indicators of high-performing teams and will allow your organization to avoid the worst outcomes of prolonged failures.
{{% /note %}}

---

#### MTTR: What the data shows

![mttr-data](/images/slides/mttr-data.png)
{.r-stretch}

###### Benchmark: 60 mins

{{% note %}}
On CircleCI, 50% of workflows recovered in 64 minutes or less, very nearly equal to our benchmark of 60 minutes. This was a significant improvement from our previous two reports, which showed median times that were 10 minutes longer, and the most notable change among any of the four metrics in this report's data. The top 25% recovered in 15 minutes or less, and the top 5% recovered in under 5 minutes. 
{{% /note %}}

---

#### Treat your default branch as the lifeblood of your project

![long live CI/CD](/images/slides/long-live-cicd.gif)
{.r-stretch}

{{% note %}}
The first step to lowering recovery times is to treat your default branch as the lifeblood of your project – and by extension, your organization. While red builds are inevitable, getting your code back to green immediately should be everyone’s top priority. With a vigilant culture in place, your organization will be poised to leverage information from your CI pipeline and remediate failures as soon as they arise.
{{% /note %}}

---

#### Getting to faster recovery times

* Treat your default branch as the lifeblood of your project
* Set up instant alerts for failed builds using services like Slack, Twilio, or Pagerduty.
* Write clear, informative error messages for your tests, allowing quick diagnosis
* Use SSH into the failed build machine to debug in the remote test environment.

{{% note %}}
Bear in mind that recovery speed is inextricably bound with pipeline duration: the shortest possible time to recovery is the length of your next pipeline run. So these techniques require the previously mentioned optimizations, and then you can start getting to faster recovery times
{{% /note %}}

---

### Success rate

_number of passing runs divided by the total number of runs over a period of time_

{{% note %}}
Success rate is another indicator, alongside mean time to recovery, of the stability of your application development process. However, the impact of success rate on both customers and development teams can vary according to a number of factors. Did the failure occur on the default branch or a development branch? Did the workflow involve a deployment? How important is the application or service being tested?
{{% /note %}}

---

![failed signals are ok](/images/slides/failed-signal-taunting.gif)
{.r-stretch}

{{% note %}}
A failed signal is not necessarily indicative that something has gone wrong or there is a problem that needs to be addressed on a deeper level than your standard recovery processes. Far more important is your team’s ability to ingest the signal quickly (duration) and remediate the error effectively (MTTR). Again, a failed workflow that delivers a fast, valuable signal is far more desirable than a passing workflow that offers thin or unreliable information. 
{{% /note %}}

---

#### Success rate benchmark

###### 90%+ success rate on default branches

{{% note %}}
We recommend maintaining a success rate of 90% or higher on default branches. This is a reasonable target for the mainline code of a mission-critical app, where changes should be merged only after passing a series of well written tests. Failures on topic branches are generally less disruptive to software delivery than those that occur on the default branch. It's important for your team to set its own benchmark for success on various other branches depending on how you use them. 
{{% /note %}}

---

#### Success rate: What the data shows

![success-rate-data](/images/slides/success-rate-data.png)
{.r-stretch}

###### Benchmark: 90%+ on default

{{% note %}}
Among CircleCI users, success rates on the default branch were 77% on average. On non-default branches, they were 67% on average. Success rates on the default branch have held steady over the past several iterations of our report. While neither number reaches our benchmark of 90%, the pattern of non-default branches having higher numbers of failures indicates that teams are utilizing effective branching patterns to isolate experimental or risky changes from critical mainline code. And while success rates haven’t moved much over the history of this report, recovery times have fallen sharply. This is a welcome sign that organizations are prioritizing iteration and resilience over momentum-killing perfectionism. 
{{% /note %}}

---

### Throughput

_average number of workflow runs that an organization completes on a given project per day_

{{% note %}}
Throughput traditionally reflects the number of changes your developers are committing to your codebase in a 24-hour period
{{% /note %}}

---

![high velocity](/images/slides/high-velocity.gif)
{.r-stretch}

{{% note %}}
It is also useful as a measurement of team flow as it tracks how many units of work move through the CI system. When performed at or above recommended levels, throughput puts the “continuous” in continuous delivery — the higher your throughput, the more frequently you are performing work on your application. 
{{% /note %}}

---

![only a model](/images/slides/only-a-model.gif)
{.r-stretch}

{{% note %}}
Of course, throughput also tells you nothing about the quality of work you are performing, so it is important to consider the richness of your test data as well as your performance on other metrics such as success rate and duration to get a complete picture. As with duration, a high throughput score means little if you are frequently pushing poor quality code to users. So what's ideal?
{{% /note %}}

---

#### Throughput benchmark

{{% fragment %}}It depends.{{% /fragment %}}

{{% note %}}
Of all the metrics, throughput is the most subjective to organizational goals. A large cloud-native organization actively developing a critical product line will require far higher levels of throughput than a small team maintaining legacy software or niche internal tooling. It really does depend. There's isn't a universally applicable throughput target - it needs to be set according to your internal business requirements. The type of work, the resources available, the expectations of your users all play into it. Far more important than the volume of work you’re doing is the quality and impact of that work. 
{{% /note %}}

---

#### Throughput: What the data shows

![throughput-data](/images/slides/throughput-data.png)
{.r-stretch}

###### Benchmark: at the speed of your business

{{% note %}}
In our data set, the median workflow ran 1.54 times per day, a slight increase from 1.43 times per day in 2022. At the upper end of the spectrum, the top 5% of workflows ran 7 times per day or more, on par with what we’ve seen in previous years. Overall, the average project had 2.93 pipeline runs in 2023 compared to 2.83 in 2022. This uptick in productivity is not especially notable, but when taken in combination with the sharp decrease in MTTR discussed earlier in the report, it may reflect that teams are committing to smaller, more frequent changes to limit the complexity of outages and achieve faster, more consistent feedback on the state of their applications. 
{{% /note %}}

---

##### Throughput is the most dependent on the other metrics

{{% note %}}
Of the four metrics measured in this report, throughput is the most dependent on the others.  How long your workflows take to complete, how often those workflows fail, and the amount of time it takes to recover from a failure all affect your developers’ ability to focus on new work and the frequency of their commits. To improve your team’s throughput, first address all the potential underlying factors that can affect team productivity.
{{% /note %}}

---

![trailing indicators](/images/slides/trailing-indicator.gif)
{.r-stretch}

{{% note %}}
Throughput is often a trailing indicator of other changes in your processes and environment. Rather than setting an arbitrary throughput goal, set a goal that reflects your business needs, capture a baseline measurement, and monitor for fluctuations that indicate changes in your team’s ability to do work. Achieving the right level of throughput means staying ahead of customer needs and competitive threats while also continuously validating the health of your application and development process. 
{{% /note %}}

---

#### High-performing teams in 2023

![high-performing teams](/images/slides/metrics-comparison.png)
{.r-stretch}

{{% note %}}
Measuring and then optimizing Duration, Throughput, Mean Time to Recovery, and Success Rate gives teams a tremendous advantage over organizations that do not track these key metrics.
{{% /note %}}

---

### Platform Teams, DevOps, and YOU

{{% note %}}
I'm sure you've all heard by now that DevOps is dead.
{{% /note %}}

---

#### No, DevOps is not dead

![devops is not dead](/images/slides/devops-not-dead.png)
{.r-stretch}

{{% note %}}
DevOps as a principle, a mindset of putting culture ahead of tools, and breaking down silos (physical and cultural) and growing lines of communication between Dev and Ops has been good. DevOps is not going anywhere, and still forms the construct for how high-performing engineering teams (and organizations) function. But at the same time, let's think back to earlier where I talked about the complexity of modern app development, specifically illustrated with the CNCF landscape.  
{{% /note %}}

---

![cncf landscape](/images/slides/cncf-landscape.png)
{.r-stretch}

{{% note %}}
There's constantly a need for devs to learn new tools and sometimes infrastructure, while coding and prioritizing ops tasks alongside feature development. The weight of these demands not only leads to lower levels of productivity and effectiveness, but it also shows up in stress, burnout, and reduced job satisfaction. And as a result, we've seen the cognitive load increase, driving up errors and negatively impacting the customer experience. So what are some of the practices your team can begin to incorporate to increase your platform’s stability, do more with less, and save money?
{{% /note %}}

---

### The Rise of Platform Teams

![platform teams](/images/slides/platform-teams.png)
{.r-stretch}

{{% note %}}
One of the things we've started seeing in the industry is a logical extension of a mature DevOps org... Platform engineering (or the Platform Team) Platform engineering is designed to work alongside existing DevOps concepts while alleviating the associated cognitive load. The general premise is to bring self-service to DevOps. 
{{% /note %}}

---

![platform](/images/slides/platform.png)
{.r-stretch}

{{% note %}}
Platform engineers abstract the complexity of common DevOps processes into an internal developer platform (IDP) that provides a standard set of tools for building and deploying applications. Platform engineering aims to enhance DevOps, not replace it, by removing the need for developers to learn, develop, and maintain infrastructure tools and processes. So let's look at how Platform engineering can contribute to achieving these metrics for high-performing engineering teams
{{% /note %}}

---

#### Platform Perspective: Duration

* Identify and eliminate impediments to developer velocity
* Set guardrails and enforce quality standards across projects
* Standardize test suites & CI pipeline configs, i.e. shareable config templates & policies
* Welcome failed pipelines, i.e. fast failure
* Actively monitor, streamline, and parallelize pipelines across the org

{{% note %}}
Duration: Developers will naturally gravitate toward speed. And while platform teams are tasked with identifying and eliminating impediments to developer velocity, that is not their only mandate. Another, perhaps more important, responsibility of the platform engineer is to set guardrails and enforce quality standards across projects. These optimizations can save you valuable developer minutes without sacrificing the quality of your builds.   
{{% /note %}}

---

#### Platform Perspective: MTTR

* Ephasise value of deploy-ready, default branches
* Set up effective monitoring and alerting systems, and track recovery time
* Limit frequency and severity of broken builds with role-based AC and config policies
* Config- and Infrastructure-as-Code tools limit potential for misconfig errors
* Actively monitor, streamline, and parallelize pipelines across the org

{{% note %}}
MTTR: Platform teams often form the bridge between an organization’s business goals and its software delivery practices. Equipping developers to recover from broken builds quickly can have a significant impact on an organization's bottom line in terms of both developer productivity and customer satisfaction. Platform engineers can improve mean time to recovery in several ways. 
{{% /note %}}

---

#### Platform Perspective: Success Rate

* With low success rates, look at MTTR and shorten recovery time first
* Set baseline success rate, then aim for continuous improvement, looking for flaky tests or gaps in test coverage
* Be mindful of patterns and influence of external factors, i.e. decline on Fridays, holidays, etc.

{{% note %}}
Success rate: It can be tempting as an organization to chase a success rate of 100% or to interpret high success rates as a sign of elite software delivery performance. And while it is desirable to maintain high rates of success on default branches, this metric means very little if you are not confident in the signal you are receiving from your CI system. Platform engineers have a responsibility to look beyond surface-level metrics and uncover the most meaningful data about team performance. 
{{% /note %}}

---

#### Platform Perspective: Throughput

* Map goals to reality of internal & external business situations
* Capture a baseline, monitor for deviations
* Alleviate as much developer cognitive load from day-to-day work

{{% note %}}
Throughput: Platform engineering exists primarily to remove blockers from development teams and to provide all the tools and resources necessary for an organization to achieve maximum productivity. Thus, throughput is often one of the top indicators used to evaluate the performance of not just the development team but of the platform team as well. 
{{% /note %}}

---

#### 2023 State of Software Delivery Report

![2023 state of software delivery report](/images/slides/sosdr-qrcode.png)
{.r-stretch}

##### circle.ci/sosdr2023}

---

{{< slide id="end" >}}
<section>
    <div class="multiCol">
        <div class="col">
            <h3 style="color: #04aa51;">Thank You.</h3>
            <p style="font-size: .75em;"></p>
            <p style="font-size: .5em;">For feedback and swag: <font style="color: rgb(111, 168, 220);">circle.ci/jeremy</font></p>
        </div>
        <div class="col" align="left" style="font-size: .5em;">
            <img src="/images/slides/polywork.png" height="50px" style="vertical-align: middle; margin: 20px;">timeline.jerdog.me<br />
            <img src="/images/slides/twitter.png" height="50px" style="vertical-align: middle; margin: 20px;">@IAmJerdog<br />
            <img src="/images/slides/devto.png" height="50px" style="vertical-align: middle; margin: 20px;">@jerdog<br />
            <img src="/images/slides/linkedin.png" height="50px" style="vertical-align: middle; margin: 20px;">/in/jeremymeiss<br />
            <img src="/images/slides/mastodon.png" height="50px" style="vertical-align: middle; margin: 20px;">@jerdog@hachyderm.io<br />
        </div>
    </div>
</section>