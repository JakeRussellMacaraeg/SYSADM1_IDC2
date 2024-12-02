<table>
<colgroup>
<col style="width: 48%" />
<col style="width: 35%" />
<col style="width: 15%" />
</colgroup>
<thead>
<tr class="header">
<th colspan="3"><p><img src="media/image2.png"
style="width:2.4in;height:0.58819in" /></p>
<p>SCHOOL OF INFORMATION AND TECHNOLOGY</p></th>
</tr>
<tr class="odd">
<th><p>NAME:</p>
<p><strong>MACARAEG, JAKE RUSSELL F.</strong></p>
<p><strong>PADILLA, ARVIN</strong></p></th>
<th><p>DATE PERFORMED:</p>
<p><strong>28/11/2024</strong></p></th>
<th rowspan="2">/50 </th>
</tr>
<tr class="header">
<th>Section: <strong>IDC2</strong></th>
<th>DATE SUBMITTED:</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# SYSADM1 -- Capacity Management & Planning {#sysadm1-capacity-management-planning}

## Part 1. A Simulated Dataset for Capacity Planning Exercise {#part-1.-a-simulated-dataset-for-capacity-planning-exercise .unnumbered}

**Scenario:** A mid-sized e-commerce website is expecting a significant
surge in traffic due to an upcoming holiday sale.

![](media/image1.png){width="4.749564741907261in"
height="2.4791666666666665in"}

### [Projected Traffic Increase]{.underline} {#projected-traffic-increase .unnumbered}

- **Expected Peak Traffic:** 5x the normal peak traffic

- **Peak Time:** 12:00 PM - 3:00 PM on the sale day

### [System Specifications]{.underline} {#system-specifications .unnumbered}

- **Server Count:** 5

- **CPU Cores per Server:** 8

- **RAM per Server:** 32GB

- **Network Bandwidth per Server:** 1Gbps

### [Additional Considerations]{.underline} {#additional-considerations .unnumbered}

- **New Product Launch:** A highly anticipated product will be released
  > during the sale.

- **Marketing Campaign:** A major marketing campaign will be launched to
  > promote the sale.

- **Potential Cyber Threats:** Increased traffic can attract malicious
  > actors.

Tasks:

1.  Review the provided server performance data and identify potential
    > bottlenecks

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>CPU Utilization</strong>:</p>
<ul>
<li><p>With 60% at highest, there’s a moderate CPU usage. Although the
servers are not currently overloaded, they could be unable to handle the
anticipated spike in traffic, particularly considering the 5x
increase.</p></li>
</ul>
<p><strong>Memory Utilization</strong>:</p>
<ul>
<li><p>70% is the peak of Memory usage, leaving some room for scaling,
but it might become a bottleneck if the traffic increase is too
large.</p></li>
</ul>
<p><strong>Network Bandwidth</strong>:</p>
<ul>
<li><p>It seems that the Network usage is sufficient for the current
needs but could be saturated with a 5x traffic increase. The servers
have 1 Gbps of bandwidth each, and with increased traffic, this could be
a potential bottleneck.</p></li>
</ul>
<p><strong>Response Time</strong>:</p>
<ul>
<li><p>Response times increase under load, which suggests that the
servers are nearing their capacity limits. This would likely worsen
during the anticipated surge.</p></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

2.  Brainstorm possible solutions to address the identified bottlenecks.
    > Propose potential solutions considering hardware and
    > software-based solutions.

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Horizontal Scaling (Adding More Servers)</strong>:</p>
<ul>
<li><p>The easiest way to tackle increased demand is to simply add more
servers. This would help distribute the load and give the system more
breathing room.</p></li>
</ul>
<p><strong>Load Balancing</strong>:</p>
<ul>
<li><p>A load balancer could be used to evenly distribute incoming
traffic across all available servers, preventing any one server from
being overwhelmed. This helps ensure a smooth user experience even
during peak times.</p></li>
</ul>
<p><strong>Network Bandwidth Optimization</strong>:</p>
<ul>
<li><p>To prevent network congestion, increasing network bandwidth or
using a network load balancer would ensure that the system can handle
the influx of data without issues.</p></li>
</ul>
<p><strong>Cloud Auto-Scaling</strong>:</p>
<ul>
<li><p>Leveraging cloud services could help by automatically adding or
removing servers based on demand. This way, you only pay for what you
need and can handle the traffic surge more effectively.</p></li>
</ul>
<p><strong>Enhanced Security Measures</strong>:</p>
<ul>
<li><p>Given the potential for malicious traffic during high-demand
periods, implementing a Web Application Firewall (WAF) or DDoS
protection could help safeguard the system from cyber threats.</p></li>
</ul>
<p><strong>Caching &amp; CDN</strong>:</p>
<ul>
<li><p>By caching content and using a Content Delivery Network (CDN),
static assets like images, scripts, and stylesheets can be offloaded to
edge servers, reducing the load on the main servers and speeding up
response times.</p></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

3.  Discuss the pros and cons of each proposed solution by filling out
    > the table below.

<table style="width:100%;">
<colgroup>
<col style="width: 14%" />
<col style="width: 30%" />
<col style="width: 17%" />
<col style="width: 17%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Proposed Solution</strong></th>
<th rowspan="7"><table>
<colgroup>
<col style="width: 47%" />
<col style="width: 52%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Pros</strong></th>
<th><strong>Cons</strong></th>
</tr>
<tr class="odd">
<th>Increases capacity easily, simple to implement.</th>
<th><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>Requires more servers, which may need additional monitoring.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
</tr>
<tr class="header">
<th>Evenly distributes traffic, prevents server overload.</th>
<th>Needs careful setup, can create a single point of failure.</th>
</tr>
<tr class="odd">
<th>Ensures sufficient bandwidth for high traffic volumes.</th>
<th>Costly for additional bandwidth.</th>
</tr>
<tr class="header">
<th>Scales automatically with traffic demands, flexible.</th>
<th>Potentially high cost; needs proper configuration.</th>
</tr>
<tr class="odd">
<th>Protects against malicious attacks, improves uptime.</th>
<th>Potentially high cost and configuration complexity.</th>
</tr>
<tr class="header">
<th>Reduces load on servers, improves response times.</th>
<th>Static content may not update instantly.</th>
</tr>
</thead>
<tbody>
</tbody>
</table></th>
<th><strong>Cost</strong></th>
<th><strong>Complexity</strong></th>
<th><strong>Potential impact on system performance</strong></th>
</tr>
<tr class="odd">
<th><em><strong>Horizontal Scaling (Adding More
Servers)</strong>:</em></th>
<th><blockquote>
<p>₱150,000–₱250,000 (for 5 servers)</p>
</blockquote></th>
<th>Medium</th>
<th><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>High; directly improves system capacity.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
</tr>
<tr class="header">
<th><em><strong>Memory Utilization</strong>:</em></th>
<th><blockquote>
<p>₱20,000–₱50,000 (load balancer software/hardware)</p>
</blockquote></th>
<th>Medium</th>
<th><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>High; ensures smoother traffic distribution.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
</tr>
<tr class="odd">
<th><em><strong>Network Bandwidth Optimization</strong>:</em></th>
<th><p>₱50,000–₱100,000 (depending on provider rates)</p>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
<th><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>Low</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
<th><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>Medium; resolves potential network bottlenecks.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
</tr>
<tr class="header">
<th><em><strong>Cloud Auto-Scaling</strong>:</em></th>
<th><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><blockquote>
<p>₱100,000–₱300,000 (based on usage)</p>
</blockquote></th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
<th>High</th>
<th><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>High; optimizes resource allocation based on traffic.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
</tr>
<tr class="odd">
<th><em><strong>Enhanced Security Measures</strong>:</em></th>
<th><blockquote>
<p>₱50,000–₱100,000 (for robust solutions)</p>
</blockquote></th>
<th>High</th>
<th><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>Medium; helps secure the system from external threats.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
</tr>
<tr class="header">
<th><em><strong>Caching &amp; CDN</strong>:</em></th>
<th><table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><blockquote>
<p>₱10,000–₱30,000 (CDN subscription or setup)</p>
</blockquote></th>
</tr>
</thead>
<tbody>
</tbody>
</table>
<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
</tbody>
</table></th>
<th>Medium</th>
<th>High; reduces server load and improves performance.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

Grading Rubric:

| Criteria                    | Excellent \| 10pts                                                                                                         | Good \| 7pts                                                            | Needs Improvement \| 4pts                                                      |
|-----------------------------|----------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|--------------------------------------------------------------------------------|
| **Problem Identification**  | Accurately identifies the primary problem and provides a detailed explanation.                                             | Identifies the main problem and provides a basic explanation.           | Identifies a problem but lacks clarity or accuracy.                            |
| **Solution Proposal**       | Proposes multiple relevant solutions and provides detailed explanations, including potential drawbacks and benefits.       | Proposes one or two relevant solutions but lacks detailed explanation.  | Proposes a solution but lacks feasibility or relevance.                        |
| **Evaluation of Solutions** | Provides a thorough evaluation of the proposed solutions, considering factors like cost, complexity, and potential impact. | Provides a basic evaluation of the proposed solutions, but lacks depth. | Does not evaluate the proposed solutions or provides a superficial evaluation. |
| Score:                      |                                                                                                                            |                                                                         | /30                                                                            |

**Part 2. Network Scalability Analysis**

Recall the e-commerce website scenario we discussed earlier. Given the
expected surge in traffic, analyze the provided network topology
diagram. Identify potential bottlenecks and areas where scalability
might be a concern. Propose specific strategies to improve the
network\'s scalability and performance to ensure a seamless user
experience during the peak traffic period. Consider factors such as
increased user demand, new applications, and security threats.

![](media/image3.png){width="5.049483814523184in"
height="3.8229166666666665in"}

| Criteria                         | Excellent \| 10pts                                                                                                                                           | Good \| 7pts                                                            | Needs Improvement \| 4pts                                                      |
|----------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|--------------------------------------------------------------------------------|
| **Network Analysis**             | Accurately identifies potential bottlenecks, security risks, and capacity limitations.                                                                       | Identifies key network components and some potential bottlenecks.       | Identifies some basic network components but lacks a comprehensive analysis.   |
| **Scalability Planning**         | Proposes multiple relevant solutions and provides detailed explanations, including potential drawbacks and benefits.                                         | Proposes some relevant scalability strategies but lacks detail.         | Proposes limited scalability strategies.                                       |
| **Evaluation of Solutions**      | Proposes comprehensive scalability strategies, including specific recommendations for hardware upgrades, software configurations, and network optimizations. | Provides a basic evaluation of the proposed solutions, but lacks depth. | Does not evaluate the proposed solutions or provides a superficial evaluation. |
| **Proposed Design**              | Provides a detailed and well-justified design, including network diagrams, configuration details, and implementation plans.                                  | Provides a basic design but lacks specific details and justifications.  | Does not provide a clear and detailed design.                                  |
| **Evaluation and Justification** | Provides a thorough evaluation of the proposed solutions, considering factors like cost, complexity, and potential impact.                                   | Provides a basic evaluation of the proposed solutions, but lacks depth. | Does not evaluate the proposed solutions or provides a superficial evaluation  |
| Score:                           |                                                                                                                                                              |                                                                         | /50                                                                            |
