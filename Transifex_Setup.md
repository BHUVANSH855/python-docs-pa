# Transifex Translator Setup & Getting Started Guide

**Project:** Punjabi (pa) Python Documentation
**Platform:** Transifex
**Audience:** Punjabi Translation Contributors

---

## 1. What You Need

You only need:

* A Transifex account
* Access to the Punjabi (pa) translation team
* Your assigned worklist
* The project Style Guide
* The project Glossary

You do **not** need:

* A GitHub fork
* A local clone of the repository
* Git/GitHub knowledge
* Pull requests

All translation work is done directly on Transifex.

---

# 2. Sign In to Transifex

Go to:

https://app.transifex.com/

Sign in using the account that was added to the Punjabi translation team.

After you are approved as a translator, the project should appear in your Transifex dashboard. Transifex's current translator documentation confirms that approved team members can access the project from their dashboard and begin translating.

---

# 3. Open the Python Documentation Project

From your Transifex dashboard:

1. Find the Python Documentation project.
2. Open the project.
3. Select the **Punjabi (pa)** language.
4. Open the resource assigned to you.

If you cannot see the Punjabi language or the assigned resource, **do not create another project or request another language**. Contact the coordinator.

---

# 4. Open the Translation Editor

Transifex provides a Web Editor where translators can work directly in their browser.

The general path is:

**Dashboard → Editor → Project → Resource → Punjabi (pa)**

Transifex's current documentation describes this as the normal way to access a resource for translation.

---

# 5. Select Your Assigned Resource

For example, if your worklist says:

`library-fileinput`

select that resource.

You will see the strings belonging to that resource.

Do not start another resource unless the coordinator asks you to.

This prevents multiple contributors from unknowingly working on the same resource.

---

# 6. Find Untranslated Strings

Once the resource is open, you will see the list of strings.

Use the:

**Untranslated**

filter/tab.

This shows strings that still need translation. Transifex provides filters such as **All**, **Untranslated**, and **Unreviewed** in the Web Editor.

---

# 7. Translate a String

Click an untranslated string.

You will see:

**Source**

The original English text.

**Translation**

The field where you enter the Punjabi translation.

Example:

Source:

`Input and Output`

Translation:

`ਇਨਪੁੱਟ ਅਤੇ ਆਉਟਪੁੱਟ`

Enter your Punjabi translation in the translation field.

---

# 8. Save the Translation

After entering your translation, use the **Save** option in the editor.

Do not assume that typing the translation automatically saves it.

Transifex allows you to save an individual translation or save multiple drafts while working.

After saving, move to the next untranslated string.

---

# 9. Important: Preserve Code and Markup

Python documentation contains technical formatting.

You may encounter things such as:

`Python`

`print()`

`os.path`

`:class:`

`:func:`

`{name}`

`%s`

```
.. code-block:: python
```

Do **not** translate or modify Python code, identifiers, Sphinx roles, placeholders, or markup unless the project guidelines specifically say otherwise.

For example:

Source:

`Use the :func:\`print` function.`

Do not change:

`:func:\`print``

Translate the surrounding natural-language text while preserving the Sphinx markup.

---

# 10. Follow the Project Glossary

Before translating technical terms, check the project's Glossary.

The glossary exists to keep terminology consistent across the entire Punjabi documentation.

If you find a technical term that is not covered by the glossary and you are unsure how it should be translated:

**Do not guess.**

Ask the coordinator.

A terminology decision can then be discussed and, if necessary, added to the glossary for future translators.

---

# 11. Follow the Style Guide

Always follow the project Style Guide when translating.

Pay particular attention to:

* Punjabi grammar
* Natural Punjabi wording
* Technical terminology
* English technical terms that should remain unchanged
* Code formatting
* Sphinx/RST markup
* Placeholders
* Consistency with existing translations

The goal is not to translate English word-for-word.

The goal is to produce **clear, natural, technically accurate Punjabi documentation**.

---

# 12. If Transifex Shows a Warning or Error

Transifex performs translation checks when translations are saved.

You may see warnings or errors related to things such as:

* Missing placeholders
* Incorrect formatting
* Variables
* Code/markup
* Numbers
* Other formatting requirements

If Transifex reports an error, read the message carefully and correct the translation before saving again. Transifex documents these checks as part of the Web Editor workflow.

If you don't understand the warning, contact the coordinator.

---

# 13. When Have You Finished a Resource?

A resource is considered ready for review when:

* All untranslated strings have been translated.
* Your translations have been saved.
* Python code and identifiers are preserved.
* Placeholders are preserved.
* RST/Sphinx markup is preserved.
* You have checked the Style Guide and Glossary.
* You have informed the coordinator.

Do not mark something as reviewed yourself unless you have been given reviewer permissions.

---

# 14. What Happens After You Finish?

Your workflow ends at Transifex.

The process is:

**Translator**

↓

Translate on Transifex

↓

Save translations

↓

**Reviewer**

↓

Review and approve

↓

**GitHub Automation**

↓

Fetch reviewed translations

↓

Update the `python-docs-pa` repository

↓

Eventually submitted upstream to CPython

You do not need to manually upload your `.po` file to GitHub.

You do not need to create a GitHub pull request.

---

# 15. What If You Get Stuck?

Please contact the coordinator if:

* You cannot find the assigned resource.
* You cannot see the Punjabi language.
* You cannot edit a string.
* A translation check fails and you don't understand why.
* A technical term is difficult to translate.
* You are unsure whether something should remain in English.
* You are unsure whether markup should be translated.
* You think a string is already translated incorrectly.
* You encounter anything that looks like a Transifex configuration problem.

**Do not create a new project, resource, language, or file to solve the problem yourself.**

---

# 16. First Translation Checklist

Before starting:

* [ ] Transifex account is activated.
* [ ] Punjabi (pa) team access is confirmed.
* [ ] Assigned worklist is available.
* [ ] Style Guide has been read.
* [ ] Glossary has been read.

While translating:

* [ ] Use the Untranslated filter.
* [ ] Translate one string at a time.
* [ ] Save translations.
* [ ] Preserve code and markup.
* [ ] Preserve placeholders.
* [ ] Follow the glossary.
* [ ] Ask the coordinator when unsure.

After finishing:

* [ ] All strings in the assigned resource are translated.
* [ ] Saved translations have been checked.
* [ ] Coordinator has been notified.
* [ ] Wait for reviewer feedback.

---

# Quick Workflow

```text
Join Punjabi Team
        ↓
Open Transifex
        ↓
Open Python Documentation Project
        ↓
Select Punjabi (pa)
        ↓
Open Assigned Resource
        ↓
Filter → Untranslated
        ↓
Translate
        ↓
Save
        ↓
Complete Resource
        ↓
Notify Coordinator
        ↓
Reviewer Reviews
        ↓
Approved Translation
        ↓
GitHub Automation
```

---

## Important

**Your job is to translate on Transifex.**

You do not need to worry about GitHub synchronization, `.po` files, commits, branches, or pull requests.

The project coordinators and automation handle the repository side after your translations have been reviewed.

If you are unsure about anything, **ask before making a change that could affect terminology or formatting.**

Welcome to the team, and thank you for helping bring Python documentation to Punjabi speakers!
