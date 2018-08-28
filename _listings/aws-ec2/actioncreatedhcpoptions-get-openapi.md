---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Create Dhcp Options
  version: 1.0.0
  description: Creates a set of DHCP options for your VPC.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AssociateDhcpOptions:
    get:
      summary: Associate Dhcp Options
      description: Associates a set of DHCP options (that you've previously created)
        with the specified VPC, or associates no DHCP options with the VPC.
      operationId: associatedhcpoptions
      x-api-path-slug: actionassociatedhcpoptions-get
      parameters:
      - in: query
        name: DhcpConfiguration.N
        description: A DHCP configuration option
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - DHCP
  /?Action=CreateDhcpOptions:
    get:
      summary: Create Dhcp Options
      description: Creates a set of DHCP options for your VPC.
      operationId: createdhcpoptions
      x-api-path-slug: actioncreatedhcpoptions-get
      parameters:
      - in: query
        name: DhcpOptionsId
        description: The ID of the DHCP options set
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      responses:
        200:
          description: OK
      tags:
      - DHCP
  /?Action=DeleteDhcpOptions:
    get:
      summary: Delete Dhcp Options
      description: Deletes the specified set of DHCP options.
      operationId: deletedhcpoptions
      x-api-path-slug: actiondeletedhcpoptions-get
      parameters:
      - in: query
        name: DhcpOptionsId.N
        description: The IDs of one or more DHCP options sets
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      responses:
        200:
          description: OK
      tags:
      - DHCP
  /?Action=DescribeDhcpOptions:
    get:
      summary: Describe Dhcp Options
      description: Describes one or more of your DHCP options sets.
      operationId: describedhcpoptions
      x-api-path-slug: actiondescribedhcpoptions-get
      parameters:
      - in: query
        name: Device
        description: The device name to expose to the instance (for example, /dev/sdh
          or        xvdh)
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: VolumeId
        description: The ID of the EBS volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - DHCP
  /?Action=ModifyVpcPeeringConnectionOptions:
    get:
      summary: Modify Vpc Peering Connection Options
      description: Modifies the VPC peering connection options on one side of a VPC
        peering connection.
      operationId: modifyvpcpeeringconnectionoptions
      x-api-path-slug: actionmodifyvpcpeeringconnectionoptions-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,       and provides an error response
        type: string
      - in: query
        name: VpcPeeringConnectionId
        description: The ID of the VPC peering connection
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC Peering Connection
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