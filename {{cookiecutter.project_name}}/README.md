[template-version]: # (0.0.2)
# {{ cookiecutter.project_name }}

**Tools**: {{ cookiecutter.tools | join(", ")}}
<br>
**Topics**: {{ cookiecutter.topics | join(", ") }}
<br>
**Industries**: {{ cookiecutter.industries | join(", ") }}

## Introduction/Overview
### Overview
{{ cookiecutter.introduction_overview }}

### Problem Context
{{ cookiecutter.problem_context }}

## Instructions

### Project Objectives
{{ cookiecutter.project_objectives }}

### General Evaluation Criteria
{{ cookiecutter.general_evaluation_criteria }}

### Notes
{{ cookiecutter.project_notes }}

## Tasks
{% for task in cookiecutter.tasks %}
### Task {{ loop.index }}: {{ task.title }}

**Time: {{ task.time }}**

{{ task.desc }}
{{ task.evaluation_criteria }}
{% endfor %}
### Optional tasks:

Here you write anything that is not stricktly required for the learning experience, but that could provide furhter insights to the learners.

## Future work

* Here you list things you think are interesting to make the lab better, but were left out due to time constrains.
