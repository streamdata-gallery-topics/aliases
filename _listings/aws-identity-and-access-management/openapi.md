swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 1
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAccountAliases:
    get:
      summary: List Account Aliases
      description: |-
        Lists the account alias associated with the AWS account (Note: you can have only
              one).
      operationId: listAccountAliases
      x-api-path-slug: actionlistaccountaliases-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Aliases
  /?Action=CreateAccountAlias:
    get:
      summary: Create Account Alias
      description: Creates an alias for your AWS account.
      operationId: createAccountAlias
      x-api-path-slug: actioncreateaccountalias-get
      parameters:
      - in: query
        name: AccountAlias
        description: The account alias to create
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Alias
  /?Action=DeleteAccountAlias:
    get:
      summary: Delete Account Alias
      description: Deletes the specified AWS account alias.
      operationId: deleteAccountAlias
      x-api-path-slug: actiondeleteaccountalias-get
      parameters:
      - in: query
        name: AccountAlias
        description: The name of the account alias to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Alias