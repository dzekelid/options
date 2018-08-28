---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Delete issue field option
  description: |-
    Deletes an option from a select list issue field.

    **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/field/{fieldKey}/option:
    get:
      summary: Get all issue field options
      description: |-
        Returns all options defined for a select list issue field. A select list issue field is a type of [issue field](https://developer.atlassian.com/cloud/jira/platform/modules/issue-field/) that allows a user to select an value from a list of options.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.getAllIssueFieldOptions_get
      x-api-path-slug: api2fieldfieldkeyoption-get
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: startAt
        description: The starting index of the returned objects
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Options
    post:
      summary: Create issue field option
      description: |-
        Creates an option for a select list issue field.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.createIssueFieldOption_post
      x-api-path-slug: api2fieldfieldkeyoption-post
      parameters:
      - in: path
        name: fieldKey
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Option
  /api/2/field/{fieldKey}/option/suggestions/edit:
    get:
      summary: Get selectable issue field options
      description: |-
        Returns options defined for a select list issue field that can be viewed and selected by the currently logged in user.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to access Jira.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.getSelectableIssueFieldOptions_get
      x-api-path-slug: api2fieldfieldkeyoptionsuggestionsedit-get
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: projectId
        description: Filters the results to options that are only available in the
          specified project
      - in: query
        name: startAt
        description: The starting index of the returned objects
      responses:
        200:
          description: OK
      tags:
      - Selectable
      - Issue
      - Field
      - Options
  /api/2/field/{fieldKey}/option/suggestions/search:
    get:
      summary: Get visible issue field options
      description: |-
        Returns options defined for a select list issue field that can be viewed by the currently logged in user.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to access Jira.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.getVisibleIssueFieldOptions_get
      x-api-path-slug: api2fieldfieldkeyoptionsuggestionssearch-get
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: projectId
        description: Filters the results to options that are only available in the
          specified project
      - in: query
        name: startAt
        description: The starting index of the returned objects
      responses:
        200:
          description: OK
      tags:
      - Visible
      - Issue
      - Field
      - Options
  /api/2/customFieldOption/{id}:
    get:
      summary: Get custom field option
      description: "Returns a custom field option. For example, an option in a cascading
        select list.  \n  \n**[Permissions](https://developer.atlassian.com/cloud/jira/platform/rest/#permissions)
        required:** None."
      operationId: com.atlassian.jira.rest.v2.issue.customfield.CustomFieldOptionResource.getCustomFieldOption_get
      x-api-path-slug: api2customfieldoptionid-get
      parameters:
      - in: path
        name: id
        description: The ID of the custom field option
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Field
      - Option
  /api/2/field/{fieldKey}/option/{optionId}:
    get:
      summary: Get issue field option
      description: |-
        Returns an option from a select list issue field.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.getIssueFieldOption_get
      x-api-path-slug: api2fieldfieldkeyoptionoptionid-get
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: path
        name: optionId
        description: The ID of the option to be returned
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Option
    put:
      summary: Update issue field option
      description: |-
        Updates an option for a select list issue field. If the option does not exist, a new option is created.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.updateIssueFieldOption_put
      x-api-path-slug: api2fieldfieldkeyoptionoptionid-put
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: path
        name: optionId
        description: The ID of the option to be updated
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Option
    delete:
      summary: Delete issue field option
      description: |-
        Deletes an option from a select list issue field.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.deleteIssueFieldOption_delete
      x-api-path-slug: api2fieldfieldkeyoptionoptionid-delete
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: path
        name: optionId
        description: The ID of the option to be deleted
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Field
      - Option
  /api/2/field/{fieldKey}/option/{optionId}/issue:
    delete:
      summary: Replace issue field option
      description: |-
        Deselects a select list issue field option in all issues that it has been selected in. A different option can be selected to replace the deselected option. The update can also be limited to a smaller set of issues by using a JQL query.

        This is an [asynchronous method](#async). The response object will contain a link to the long-running task. For example, _https://your-domain.atlassian.net/rest/api/2/task/10127_.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission. Jira permissions are not required for the app providing the field.
      operationId: com.atlassian.jira.rest.v2.issue.field.IssueFieldOptionResource.replaceIssueFieldOption_delete
      x-api-path-slug: api2fieldfieldkeyoptionoptionidissue-delete
      parameters:
      - in: path
        name: fieldKey
        description: 'The field key is specified in the following format: **$(app-key)__$(field-key)**'
      - in: query
        name: jql
        description: A JQL query that specifies the issues to be updated
      - in: path
        name: optionId
        description: The ID of the option to be deselected
      - in: query
        name: replaceWith
        description: The ID of the option that will replace the currently selected
          option
      responses:
        200:
          description: OK
      tags:
      - Replace
      - Issue
      - Field
      - Option
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---