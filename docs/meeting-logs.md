# Meeting logs

Onboarding meetings with Yenifer Hernandez. Newest first. Add the next log below this intro, above older entries.

## 2026-09-24: Yenifer / Joey

**When:** Thursday, September 24, 2026, 11:30 AM CDT  
**Attendees:** Joey Rahman, Yenifer Hernandez

### Onboarding progress

- Met nearly all engineers across the India, Egypt, and Argentina teams.
- Mahmoud Gad meeting still pending, scheduled for Friday.
- Common themes from the 1:1s:
  - Highlights: community, collaboration, teamwork.
  - Opportunities: clearer requirements, better project planning, stronger technical documentation, shorter or rotating demos.
- Carl’s office hours are highly valued. Shared Upland experience has been a bonding factor.
- Certificate management service stress-testing ticket is in progress.
  - PR target: Friday, September 25; latest Monday, September 28.

### Dashboard access and product context

- The current dashboard link is org 60 (localyticsorg), not NeutroCheck.
  - Audiences and live monitor are fine to explore freely.
- NeutroCheck (org ~3,860) needs separate access. Joey is provisioning it for Yenifer and Wanhao.
- A web SDK exists but was never shipped. No customers use it today.
- Web and mobile data integration is a possible FDE opportunity.
  - Approach Derick carefully. Likely pushback: unclear customer benefit, the effort to grant data access, and no defined success metric.

### Sprint process and the 90-day plan

- Story points are 1, 2, 3, or 5 only. Engineers split anything larger than 5.
- Completion rate matters more than total points, and points are not tied to performance review.
- Every story needs an epic, and epics link to OKRs.
- Juan runs or attends standups and grooming.
- Keep the 90-day plan updated, especially when Derick pulls Yenifer into customer meetings.
  - No need to log 1:1 summaries in the plan. Progress is shared in these calls.
- The sprint process doc in Confluence was wiped and needs to be restored before it is shared.
- Granola access for customer meeting transcripts will go through Julian.

### Next steps

- [ ] Get Yenifer and Wanhao access to NeutroCheck (org ~3,860) (Joey)
- [ ] Restore and share the sprint process doc from Confluence (Joey)
- [ ] Arrange Granola access for Yenifer via Julian (Joey)
- [ ] Submit the PR for certificate management service stress testing (Yenifer)

## 2026-09-22: Yenifer / Joey

**When:** Tuesday, September 22, 2026, 3:30 PM CDT  
**Attendees:** Joey Rahman, Yenifer Hernandez

### Onboarding progress: day 2

- SSH is set up and the Rails repo is cloned.
- Logged into the Localytics dashboard.
- “Localytics org 60” in the 90-day plan is the dashboard, not a GitHub org. It lives under the Localytics org.
- Messaged Carl about which repos to clone for full dashboard access. Response expected Wednesday.
- Met Pedro, JuanJo, Javier, and Sarah. Jigar was a no-show; reschedule for later in the week.
- Wednesday 1:1s set with Ayan, Hitesh, Saranya, Shreenath, Julian, and Abraam.
- First code ship destination is Carl’s call: the new agent repo, or the legacy platform.

### Schedule

- Juan’s NutriTech deliverable brainstorm at 1:00 PM ET Wednesday conflicts with the new-hire meeting.
  - Prioritize NutriTech. Move the new-hire meeting to Thursday.
  - Joey will coordinate the reschedule with Sarah.
- Thursday 9:00–10:20 AM is blocked on the calendar as a public personal appointment.

### Month 1 priorities

- AI agent benchmarking framework, in close collaboration with Juan (head of product) and Pedro.
  - Pedro is building an analyst agent that queries Snowflake. It needs testing and an eval framework.
- QVC engagement is not in the 90-day plan: Airtable-to-Localytics campaign integration.
  - The FDE will be Yenifer or Joey. Solution design with Carl.
  - No AI component. It is an integration project.
- Assessment agent: tooling to score customers on AI readiness. A priority for Juan.

### People to connect with

- Derick: longest tenure, deep knowledge of customer use cases.
- Mahmoud Gad (support, Egypt): best source for typical customer Snowflake query patterns, useful for analyst agent eval design.
- Emily (support, US): similar customer query knowledge.

### Tools and access

- Langfuse: request access via Julian.
- SigNoz (observability, like Datadog or Grafana): check SSO first, then ask Carl if access is missing.
  - Monitors known metrics and logs defined in code.
  - Honeybadger handles unknown exceptions and alerts on error patterns.
- Skip Confluence docs older than a year.

### Next steps

- [ ] Reschedule the new-hire meeting with Sarah (Joey)
- [ ] Request Langfuse access via Julian; check SSO for SigNoz, then ask Carl if needed (Yenifer)
- [ ] Confirm the first code ship destination with Carl (Yenifer)

## 2026-09-21: Welcome to Localytics (Yenifer / Joey)

**When:** Monday, September 21, 2026, 10:00 AM CDT  
**Attendees:** Joey Rahman, Yenifer Hernandez

### Tool access and setup

- Access confirmed: Jira, Confluence, Honeybadger, AWS (sandbox), Snowflake (sandbox), Slack, GitHub, Cursor.
- Postman can wait. Cursor is needed now.
- Still needed: admin access to org 60 (ask Julian).
- Added to the Localytics Engineering Slack channel.
- 90-day plan repo shared via Slack.

### Team and contacts

- Carl: onboarding buddy and primary contact for the first month. Technical and architecture questions.
- Juan: head of product. Roadmap questions.
- Derick: customer use cases and solutions. Hold off until week 2 or 3.
- Sarah: head of people. Escalation for unresolved HR or team questions.
- Pedro: Spain, working on the Analyst Agent (LLM querying Snowflake via SQL).
- Abraam: cloud DevOps, Egypt. Mahmoud Gad: support, also Egypt.
- Argentina: Julian (IT), JuanJo (new ML engineer, started the same day), Javier (started the week before).
- More than half of engineering is in India. Overlap may mean starting as early as 8:00 AM ET some days.

### Week 1 and week 2

- Week 1:
  - Explore org 60, the internal production test bed.
  - Study architecture with Carl: key components and current agents.
  - Meet as many teammates as possible. Target half of engineering.
  - Ship a first change, even a comment, to learn the deploy process. Use Argo CD, not GoCD.
- Week 2:
  - Keep using org 60.
  - Get acquainted with Quill: architecture, usage, and API surface.
  - Run the weekly agent metrics review (next Tuesday).
  - Take over the agent evaluation framework from Saranya. It covers eval for Quill and Analyst Agent workflows.

### Working norms

- Overcommunicate for the first 90 days. Slack, tag people, and schedule time freely.
- Ownership means shepherding work end to end: reading PRDs, breaking down tasks, deploying, monitoring, and driving adoption.
- Flag risks early. Silence on a missed commitment is the integrity failure.
- Video on for meetings is strongly recommended.
- Prefer public Slack channels over DMs after the first two weeks. DMs are fine early and for sensitive topics.
- Longer-term role is a force multiplier. The first months are focused on agents.
- AI enablement sharing session: a presentation for non-engineers is encouraged in month 1 or 2.

### Next steps

- [ ] Send Carl the 90-day plan repo link (Yenifer)
- [ ] Request admin access to org 60 from Julian (Yenifer)
- [ ] Remove the duplicate Learn and Share calendar invite (Joey)
- [ ] Send Yenifer the all-hands invite for September 30 (Joey)
