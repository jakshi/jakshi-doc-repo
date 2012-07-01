In a perfect world, where things are done well, not just quickly, I would expect to find the following when joining the company:

**Documentation**

   * Accurate / up-to-date systems architecture diagram
   * Accurate / up-to-date network diagram

   * Out-of-hours support plan

   * Incident management plan

   * Change management plan 
   * Application documentation

**Metric collection:**

   * comprehensive system metrics (eg. cpu, load, mem, disk, network, etc)

   * application metrics instrumented in code (eg. queue length, time to post new job) [statsd]

   * business metrics instrumented in code as well (eg. registrations) [statsd]
   * include network devices (eg. firewall, loadbalancers, switches, vpns, vpc)

   * include storage (eg. netapp)

   * include database

   * include cron jobs

   * include CD pipeline systems/applications (e.g., jenkins, chef, build / test farm)
   * majority of monitoring from internal systems

   * also monitor from external systems (e.g., Nimsoft/Watchmouse)

   * retrieve external monitoring data into internal collection for correlation

**Alert system:**

   * alert off data collected (passive)

   * alert on checks (active)

   * call-out on important alerts

   * email, irc/chat, sms, mobile escalation

   * call-out rotation, escalation plans

**Dashboards:**

   * Real-time dashboards of all services
   * Real-time dashboard of what is being viewed on the site, where traffic is coming from

   * Dashboards to include event / deploy lines

   * Anyone can create/share dashboards

   * No passwords to access dashboards

   * Key dashboards visible in the office on screen
   * Dashboard of environments - what's deployed
   * Cost dashboard (IaaS, SaaS)

**Correlation / Investigation**


   * Graphing system which allows ad-hoc metric correlation (eg. Graphite)

   * Centralized logging with search (eg. Logstash, Greylog)
   * Record of everything that has changed, by whom, when, and what the change was
   * Access to all relevant systems 

**Infrastructure as Code**

   * Infrastructure DB with API (Chef server)
   * All infra changes tracked, done via configuration management

**Security**


   * Automated view of what needs to be patched/updated
   * Regular vulnerability scans with recorded history
   * ssh-key as only authentication
   * segregated environments (dev, test, prod)
   * data anonymisation for performance testing

**Performance testing**

   * Prod-like environment to test in
   * Good performance test, with assumptions and approximations documented
   * Record of all previous test results
   * Automated running of test
   * Automated comparison of test results with previous tests

**Communications**

   * whole company using the same instant messaging / chat system
   * task/kanbansystem for giving work to systems engineers / infrastructure developers
   * ops twitter
   * ops status (eg. etsystatus.com; stashboard; amazon status)

**Deployment**

   * single-click deploy
   * rollback-able
   * performed by developer
   * dashboard/KPI used to validate release
   * zero-down time
   * dark-launches
   * feature flags can be turned on/off via webui

**Standards**


   * Published standards of web systems requirements

**Process**


   * Light-weight post-mortem process, blame-free
   * Daily operations review
   * Monthly/quarterly architecture summit
   * Daily stand-ups
   * Iteration planning/review
   * Regular capacity planning /cost optimization

**Meta-metrics**

   * MTTD
   * MTTR
   * Availability
   * Service degradation (Slow versus broken; features disabled to protect site)
   * CD Pipeline Availability
   * Release tracking (type, success/failure, success rate, length of incident)
