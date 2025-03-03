---
title: Managing labels
intro: 'You can classify {% ifversion fpt %}issues, pull requests, and discussions{% else %}issues and pull requests{% endif %} by creating, editing, applying, and deleting labels.'
permissions: '{% data reusables.enterprise-accounts.emu-permission-repo %}'
redirect_from:
  - /github/managing-your-work-on-github/managing-your-work-with-issues-and-pull-requests/managing-labels
  - /articles/managing-Labels
  - /articles/labeling-issues-and-pull-requests
  - /github/managing-your-work-on-github/labeling-issues-and-pull-requests
  - /articles/about-labels
  - /github/managing-your-work-on-github/about-labels
  - /articles/creating-and-editing-labels-for-issues-and-pull-requests
  - /articles/creating-a-label
  - /github/managing-your-work-on-github/creating-a-label
  - /articles/customizing-issue-labels/
  - /articles/applying-labels-to-issues-and-pull-requests
  - /github/managing-your-work-on-github/applying-labels-to-issues-and-pull-requests
  - /articles/editing-a-label
  - /github/managing-your-work-on-github/editing-a-label
  - /articles/deleting-a-label
  - /github/managing-your-work-on-github/deleting-a-label
  - /github/managing-your-work-on-github/managing-labels
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
topics:
  - Pull requests
---
  ## About labels

You can manage your work on {% data variables.product.product_name %} by creating labels to categorize {% ifversion fpt %}issues, pull requests, and discussions{% else %}issues and pull requests{% endif %}. You can apply labels in the repository the label was created in. Once a label exists, you can use the label on any {% ifversion fpt %}issue, pull request, or discussion{% else %}issue or pull request{% endif %} within that repository.

## About default labels

{% data variables.product.product_name %} provides default labels in every new repository. You can use these default labels to help create a standard workflow in a repository.

| Label              | Description                                                                                                                              |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------- |
| `bug`              | Indicates an unexpected problem or unintended behavior{% ifversion fpt or ghes %}
| `документация`     | Indicates a need for improvements or additions to documentation{% endif %}
| `duplicate`        | Indicates similar {% ifversion fpt %}issues, pull requests, or discussions{% else %}issues or pull requests{% endif %}
| `enhancement`      | Indicates new feature requests                                                                                                           |
| `good first issue` | Indicates a good issue for first-time contributors                                                                                       |
| `help wanted`      | Indicates that a maintainer wants help on an issue or pull request                                                                       |
| `invalid`          | Indicates that an {% ifversion fpt %}issue, pull request, or discussion{% else %}issue or pull request{% endif %} is no longer relevant  |
| `question`         | Indicates that an {% ifversion fpt %}issue, pull request, or discussion{% else %}issue or pull request{% endif %} needs more information |
| `wontfix`          | Indicates that work won't continue on an {% ifversion fpt %}issue, pull request, or discussion{% else %}issue or pull request{% endif %}

Default labels are included in every new repository when the repository is created, but you can edit or delete the labels later.

Issues with the `good first issue` label are used to populate the repository's `contribute` page. For an example of a `contribute` page, see [github/docs/contribute](https://github.com/github/docs/contribute).

{% ifversion fpt or ghes %}
Organization owners can customize the default labels for repositories in their organization. For more information, see "[Managing default labels for repositories in your organization](/articles/managing-default-labels-for-repositories-in-your-organization)."
{% endif %}

## Creating a label

Anyone with write access to a repository can create a label.

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-issue-pr %}
{% data reusables.project-management.labels %}
4. To the right of the search field, click **New label**.
{% data reusables.project-management.name-label %}
{% data reusables.project-management.label-description %}
{% data reusables.project-management.label-color-randomizer %}
{% data reusables.project-management.create-label %}

## Applying a label

Anyone with triage access to a repository can apply and dismiss labels.

1. Navigate to the {% ifversion fpt %}issue, pull request, or discussion{% else %}issue or pull request{% endif %}.
1. In the right sidebar, to the right of "Labels", click {% octicon "gear" aria-label="The gear icon" %}, then click a label. !["Labels" drop-down menu](/assets/images/help/issues/labels-drop-down.png)

## Editing a label

Anyone with write access to a repository can edit existing labels.

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-issue-pr %}
{% data reusables.project-management.labels %}
{% data reusables.project-management.edit-label %}
{% data reusables.project-management.name-label %}
{% data reusables.project-management.label-description %}
{% data reusables.project-management.label-color-randomizer %}
{% data reusables.project-management.save-label %}

## Deleting a label

Anyone with write access to a repository can delete existing labels.

Deleting a label will remove the label from issues and pull requests.

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-issue-pr %}
{% data reusables.project-management.labels %}
{% data reusables.project-management.delete-label %}

## Дополнительная литература
- "[Filtering and searching issues and pull requests](/issues/tracking-your-work-with-issues/filtering-and-searching-issues-and-pull-requests)"{% ifversion fpt or ghes %}
- "[Managing default labels for repositories in your organization](/articles/managing-default-labels-for-repositories-in-your-organization)"{% endif %}{% ifversion fpt %}
- "[Encouraging helpful contributions to your project with labels](/communities/setting-up-your-project-for-healthy-contributions/encouraging-helpful-contributions-to-your-project-with-labels)"{% endif %}
