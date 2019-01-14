{% macro show_main_text() %}
<div id="main">

<img src="{{baseUrl}}/admin/images/toolsList.png" style="width: 700px"><br>

**Learning Management System**: This module website is the main source of information for the module. In addition, we use LumiNUS for some things %%(e.g., announcements, file submissions, grade book, ...)%%.

**Collaboration platform**: You are ==_required to_ use GitHub== as the hosting and collaboration platform of your project (i.e., to hold the Code repository, Issue Tracker, etc.). See [Appendix E]({{baseUrl}}/admin/index.html#admin-appendixE-github) for more info on how to setup and use GitHub for your project.

<div id="communication">

**Communication**: Keeping a record of communications among your team can help you, and us, in many ways. We encourage you to do at least some of the project communication in written medium (e.g., GitHub Issue Tracker) to practice how to communicate technical things in written form.
 * Instead of the LumiNUS forum, we encourage you to ==post your questions/suggestions in this [github/nus-{{ module | lower }}-{{ semester }}/forum]({{module_org}}/forum/issues)==.
 * Alternatively, you can post in our slack channel [{{slack_team}}]({{slack_team}}). We encourage you all to ==join the slack channel== (you'll need to use an email address ending in `@nus.edu.sg`, `@comp.nus.edu.sg`, `@u.nus.edu.sg` or `@u.nus.edu` to join this channel).
 * Note that slack is useful for quick chats while issue tracker is useful for longer-running conversations. GitHub forum posts will not appear in slack (or vice-versa). 
 * Later on, you may create a channel for your own team in slack. 
 
</div>

**IDE**: You are recommended to use [Intellij IDEA](https://www.jetbrains.com/idea/) for module-related programming work. You may use the community edition (free) or the ultimate edition (free for students). While the use of Intellij is not compulsory, note that module materials are optimized for Intellij. Use other IDEs at your own risk. 

**Revision control**: You are ==_required to_ use Git==. Other revision control software are not allowed.  
The recommended GUI client for Git is [SourceTree](https://www.sourcetreeapp.com/) (which comes bundled with Git), but you may use any other, or none.

**Analyzing code authorship**: We use a custom-built tool called [RepoSense](https://github.com/reposense/RepoSense) for extracting code written by each person.

<div class="indented-level2">
<panel type="seamless" header="##### Using RepoSense">
  <include src="reposenseCompatibility.md#main" />
</panel>
</div>

</div>
{% endmacro %}

{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("tools", show_main_text) }}