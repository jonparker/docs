---
title: Module applicationloadbalancing
---

<a href="../index.html">@pulumi/aws</a> &gt; applicationloadbalancing

<h2 class="pdoc-module-header">Index</h2>

* <a href="#Listener">class Listener</a>
* <a href="#ListenerCertificate">class ListenerCertificate</a>
* <a href="#ListenerRule">class ListenerRule</a>
* <a href="#LoadBalancer">class LoadBalancer</a>
* <a href="#TargetGroup">class TargetGroup</a>
* <a href="#TargetGroupAttachment">class TargetGroupAttachment</a>
* <a href="#getListener">function getListener</a>
* <a href="#getLoadBalancer">function getLoadBalancer</a>
* <a href="#getTargetGroup">function getTargetGroup</a>
* <a href="#GetListenerArgs">interface GetListenerArgs</a>
* <a href="#GetListenerResult">interface GetListenerResult</a>
* <a href="#GetLoadBalancerArgs">interface GetLoadBalancerArgs</a>
* <a href="#GetLoadBalancerResult">interface GetLoadBalancerResult</a>
* <a href="#GetTargetGroupArgs">interface GetTargetGroupArgs</a>
* <a href="#GetTargetGroupResult">interface GetTargetGroupResult</a>
* <a href="#ListenerArgs">interface ListenerArgs</a>
* <a href="#ListenerCertificateArgs">interface ListenerCertificateArgs</a>
* <a href="#ListenerCertificateState">interface ListenerCertificateState</a>
* <a href="#ListenerRuleArgs">interface ListenerRuleArgs</a>
* <a href="#ListenerRuleState">interface ListenerRuleState</a>
* <a href="#ListenerState">interface ListenerState</a>
* <a href="#LoadBalancerArgs">interface LoadBalancerArgs</a>
* <a href="#LoadBalancerState">interface LoadBalancerState</a>
* <a href="#TargetGroupArgs">interface TargetGroupArgs</a>
* <a href="#TargetGroupAttachmentArgs">interface TargetGroupAttachmentArgs</a>
* <a href="#TargetGroupAttachmentState">interface TargetGroupAttachmentState</a>
* <a href="#TargetGroupState">interface TargetGroupState</a>

<a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts">applicationloadbalancing/getListener.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts">applicationloadbalancing/getLoadBalancer.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts">applicationloadbalancing/getTargetGroup.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts">applicationloadbalancing/listener.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts">applicationloadbalancing/listenerCertificate.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts">applicationloadbalancing/listenerRule.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts">applicationloadbalancing/loadBalancer.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts">applicationloadbalancing/targetGroup.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts">applicationloadbalancing/targetGroupAttachment.ts</a> 


<h2 class="pdoc-module-header" id="Listener">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L12">class Listener</a>
</h2>

Provides a Load Balancer Listener resource.

~> **Note:** `aws_alb_listener` is known as `aws_lb_listener`. The functionality is identical.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L52">constructor</a>
</h3>

```typescript
new Listener(name: string, args: ListenerArgs, opts?: pulumi.CustomResourceOptions)
```


Create a Listener resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L21">method get</a>
</h3>

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: ListenerState): Listener
```


Get an existing Listener resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L13">method getProvider</a>
</h3>

```typescript
getProvider(moduleMember: string): ProviderResource | undefined
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L85">method isInstance</a>
</h3>

```typescript
static isInstance(obj: any): boolean
```


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L28">property arn</a>
</h3>

```typescript
public arn: pulumi.Output<string>;
```


The ARN of the listener (matches `id`)

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L32">property certificateArn</a>
</h3>

```typescript
public certificateArn: pulumi.Output<string | undefined>;
```


The ARN of the default SSL server certificate. Exactly one certificate is required if the protocol is HTTPS. For adding additional SSL certificates, see the [`aws_lb_listener_certificate` resource](https://www.terraform.io/docs/providers/aws/r/lb_listener_certificate.html).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L36">property defaultAction</a>
</h3>

```typescript
public defaultAction: pulumi.Output<{ ... }>;
```


An Action block. Action blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L80">property id</a>
</h3>

```typescript
id: Output<ID>;
```


id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L40">property loadBalancerArn</a>
</h3>

```typescript
public loadBalancerArn: pulumi.Output<string>;
```


The ARN of the load balancer.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L44">property port</a>
</h3>

```typescript
public port: pulumi.Output<number>;
```


The port. Specify a value from `1` to `65535` or `#{port}`. Defaults to `#{port}`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L48">property protocol</a>
</h3>

```typescript
public protocol: pulumi.Output<string | undefined>;
```


The protocol. Valid values are `HTTP`, `HTTPS`, or `#{protocol}`. Defaults to `#{protocol}`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L52">property sslPolicy</a>
</h3>

```typescript
public sslPolicy: pulumi.Output<string>;
```


The name of the SSL Policy for the listener. Required if `protocol` is `HTTPS`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L11">property urn</a>
</h3>

```typescript
urn: Output<URN>;
```


urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

<h2 class="pdoc-module-header" id="ListenerCertificate">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L14">class ListenerCertificate</a>
</h2>

Provides a Load Balancer Listener Certificate resource.

This resource is for additional certificates and does not replace the default certificate on the listener.

~> **Note:** `aws_alb_listener_certificate` is known as `aws_lb_listener_certificate`. The functionality is identical.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L34">constructor</a>
</h3>

```typescript
new ListenerCertificate(name: string, args: ListenerCertificateArgs, opts?: pulumi.CustomResourceOptions)
```


Create a ListenerCertificate resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L23">method get</a>
</h3>

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: ListenerCertificateState): ListenerCertificate
```


Get an existing ListenerCertificate resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L13">method getProvider</a>
</h3>

```typescript
getProvider(moduleMember: string): ProviderResource | undefined
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L85">method isInstance</a>
</h3>

```typescript
static isInstance(obj: any): boolean
```


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L30">property certificateArn</a>
</h3>

```typescript
public certificateArn: pulumi.Output<string>;
```


The ARN of the certificate to attach to the listener.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L80">property id</a>
</h3>

```typescript
id: Output<ID>;
```


id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L34">property listenerArn</a>
</h3>

```typescript
public listenerArn: pulumi.Output<string>;
```


The ARN of the listener to which to attach the certificate.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L11">property urn</a>
</h3>

```typescript
urn: Output<URN>;
```


urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

<h2 class="pdoc-module-header" id="ListenerRule">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L12">class ListenerRule</a>
</h2>

Provides a Load Balancer Listener Rule resource.

~> **Note:** `aws_alb_listener_rule` is known as `aws_lb_listener_rule`. The functionality is identical.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L44">constructor</a>
</h3>

```typescript
new ListenerRule(name: string, args: ListenerRuleArgs, opts?: pulumi.CustomResourceOptions)
```


Create a ListenerRule resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L21">method get</a>
</h3>

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: ListenerRuleState): ListenerRule
```


Get an existing ListenerRule resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L13">method getProvider</a>
</h3>

```typescript
getProvider(moduleMember: string): ProviderResource | undefined
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L85">method isInstance</a>
</h3>

```typescript
static isInstance(obj: any): boolean
```


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L28">property actions</a>
</h3>

```typescript
public actions: pulumi.Output<{ ... }[]>;
```


An Action block. Action blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L32">property arn</a>
</h3>

```typescript
public arn: pulumi.Output<string>;
```


The ARN of the rule (matches `id`)

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L36">property conditions</a>
</h3>

```typescript
public conditions: pulumi.Output<{ ... }[]>;
```


A Condition block. Condition blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L80">property id</a>
</h3>

```typescript
id: Output<ID>;
```


id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L40">property listenerArn</a>
</h3>

```typescript
public listenerArn: pulumi.Output<string>;
```


The ARN of the listener to which to attach the rule.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L44">property priority</a>
</h3>

```typescript
public priority: pulumi.Output<number>;
```


The priority for the rule between `1` and `50000`. Leaving it unset will automatically set the rule with next available priority after currently existing highest rule. A listener can't have multiple rules with the same priority.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L11">property urn</a>
</h3>

```typescript
urn: Output<URN>;
```


urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

<h2 class="pdoc-module-header" id="LoadBalancer">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L12">class LoadBalancer</a>
</h2>

Provides a Load Balancer resource.

~> **Note:** `aws_alb` is known as `aws_lb`. The functionality is identical.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L103">constructor</a>
</h3>

```typescript
new LoadBalancer(name: string, args?: LoadBalancerArgs, opts?: pulumi.CustomResourceOptions)
```


Create a LoadBalancer resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L21">method get</a>
</h3>

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: LoadBalancerState): LoadBalancer
```


Get an existing LoadBalancer resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L13">method getProvider</a>
</h3>

```typescript
getProvider(moduleMember: string): ProviderResource | undefined
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L85">method isInstance</a>
</h3>

```typescript
static isInstance(obj: any): boolean
```


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L28">property accessLogs</a>
</h3>

```typescript
public accessLogs: pulumi.Output<{ ... }>;
```


An Access Logs block. Access Logs documented below. Only valid for Load Balancers of type `application`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L32">property arn</a>
</h3>

```typescript
public arn: pulumi.Output<string>;
```


The ARN of the load balancer (matches `id`).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L36">property arnSuffix</a>
</h3>

```typescript
public arnSuffix: pulumi.Output<string>;
```


The ARN suffix for use with CloudWatch Metrics.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L40">property dnsName</a>
</h3>

```typescript
public dnsName: pulumi.Output<string>;
```


The DNS name of the load balancer.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L45">property enableCrossZoneLoadBalancing</a>
</h3>

```typescript
public enableCrossZoneLoadBalancing: pulumi.Output<boolean | undefined>;
```


If true, cross-zone load balancing of the load balancer will be enabled.
This is a `network` load balancer feature. Defaults to `false`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L50">property enableDeletionProtection</a>
</h3>

```typescript
public enableDeletionProtection: pulumi.Output<boolean | undefined>;
```


If true, deletion of the load balancer will be disabled via
the AWS API. This will prevent Terraform from deleting the load balancer. Defaults to `false`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L54">property enableHttp2</a>
</h3>

```typescript
public enableHttp2: pulumi.Output<boolean | undefined>;
```


Indicates whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L80">property id</a>
</h3>

```typescript
id: Output<ID>;
```


id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L58">property idleTimeout</a>
</h3>

```typescript
public idleTimeout: pulumi.Output<number | undefined>;
```


The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L62">property internal</a>
</h3>

```typescript
public internal: pulumi.Output<boolean>;
```


If true, the LB will be internal.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L66">property ipAddressType</a>
</h3>

```typescript
public ipAddressType: pulumi.Output<string>;
```


The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L70">property loadBalancerType</a>
</h3>

```typescript
public loadBalancerType: pulumi.Output<string | undefined>;
```


The type of load balancer to create. Possible values are `application` or `network`. The default value is `application`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L76">property name</a>
</h3>

```typescript
public name: pulumi.Output<string>;
```


The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
Terraform will autogenerate a name beginning with `tf-lb`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L80">property namePrefix</a>
</h3>

```typescript
public namePrefix: pulumi.Output<string | undefined>;
```


Creates a unique name beginning with the specified prefix. Conflicts with `name`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L84">property securityGroups</a>
</h3>

```typescript
public securityGroups: pulumi.Output<string[]>;
```


A list of security group IDs to assign to the LB. Only valid for Load Balancers of type `application`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L88">property subnetMappings</a>
</h3>

```typescript
public subnetMappings: pulumi.Output<{ ... }[]>;
```


A subnet mapping block as documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L94">property subnets</a>
</h3>

```typescript
public subnets: pulumi.Output<string[]>;
```


A list of subnet IDs to attach to the LB. Subnets
cannot be updated for Load Balancers of type `network`. Changing this value
for load balancers of type `network` will force a recreation of the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L98">property tags</a>
</h3>

```typescript
public tags: pulumi.Output<{ ... } | undefined>;
```


A mapping of tags to assign to the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L11">property urn</a>
</h3>

```typescript
urn: Output<URN>;
```


urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L99">property vpcId</a>
</h3>

```typescript
public vpcId: pulumi.Output<string>;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L103">property zoneId</a>
</h3>

```typescript
public zoneId: pulumi.Output<string>;
```


The canonical hosted zone ID of the load balancer (to be used in a Route 53 Alias record).

<h2 class="pdoc-module-header" id="TargetGroup">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L12">class TargetGroup</a>
</h2>

Provides a Target Group resource for use with Load Balancer resources.

~> **Note:** `aws_alb_target_group` is known as `aws_lb_target_group`. The functionality is identical.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L85">constructor</a>
</h3>

```typescript
new TargetGroup(name: string, args: TargetGroupArgs, opts?: pulumi.CustomResourceOptions)
```


Create a TargetGroup resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L21">method get</a>
</h3>

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: TargetGroupState): TargetGroup
```


Get an existing TargetGroup resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L13">method getProvider</a>
</h3>

```typescript
getProvider(moduleMember: string): ProviderResource | undefined
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L85">method isInstance</a>
</h3>

```typescript
static isInstance(obj: any): boolean
```


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L28">property arn</a>
</h3>

```typescript
public arn: pulumi.Output<string>;
```


The ARN of the Target Group (matches `id`)

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L32">property arnSuffix</a>
</h3>

```typescript
public arnSuffix: pulumi.Output<string>;
```


The ARN suffix for use with CloudWatch Metrics.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L36">property deregistrationDelay</a>
</h3>

```typescript
public deregistrationDelay: pulumi.Output<number | undefined>;
```


The amount time for Elastic Load Balancing to wait before changing the state of a deregistering target from draining to unused. The range is 0-3600 seconds. The default value is 300 seconds.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L40">property healthCheck</a>
</h3>

```typescript
public healthCheck: pulumi.Output<{ ... }>;
```


A Health Check block. Health Check blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L80">property id</a>
</h3>

```typescript
id: Output<ID>;
```


id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L44">property name</a>
</h3>

```typescript
public name: pulumi.Output<string>;
```


The name of the target group. If omitted, Terraform will assign a random, unique name.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L48">property namePrefix</a>
</h3>

```typescript
public namePrefix: pulumi.Output<string | undefined>;
```


Creates a unique name beginning with the specified prefix. Conflicts with `name`. Cannot be longer than 6 characters.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L52">property port</a>
</h3>

```typescript
public port: pulumi.Output<number>;
```


The port to use to connect with the target. Valid values are either ports 1-65536, or `traffic-port`. Defaults to `traffic-port`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L56">property protocol</a>
</h3>

```typescript
public protocol: pulumi.Output<string>;
```


The protocol to use to connect with the target. Defaults to `HTTP`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L60">property proxyProtocolV2</a>
</h3>

```typescript
public proxyProtocolV2: pulumi.Output<boolean | undefined>;
```


Boolean to enable / disable support for proxy protocol v2 on Network Load Balancers. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/load-balancer-target-groups.html#proxy-protocol) for more information.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L64">property slowStart</a>
</h3>

```typescript
public slowStart: pulumi.Output<number | undefined>;
```


The amount time for targets to warm up before the load balancer sends them a full share of requests. The range is 30-900 seconds or 0 to disable. The default value is 0 seconds.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L68">property stickiness</a>
</h3>

```typescript
public stickiness: pulumi.Output<{ ... }>;
```


A Stickiness block. Stickiness blocks are documented below. `stickiness` is only valid if used with Load Balancers of type `Application`

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L72">property tags</a>
</h3>

```typescript
public tags: pulumi.Output<{ ... } | undefined>;
```


A mapping of tags to assign to the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L81">property targetType</a>
</h3>

```typescript
public targetType: pulumi.Output<string | undefined>;
```


The type of target that you must specify when registering targets with this target group.
The possible values are `instance` (targets are specified by instance ID) or `ip` (targets are specified by IP address).
The default is `instance`. Note that you can't specify targets for a target group using both instance IDs and IP addresses.
If the target type is `ip`, specify IP addresses from the subnets of the virtual private cloud (VPC) for the target group,
the RFC 1918 range (10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16), and the RFC 6598 range (100.64.0.0/10).
You can't specify publicly routable IP addresses.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L11">property urn</a>
</h3>

```typescript
urn: Output<URN>;
```


urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L85">property vpcId</a>
</h3>

```typescript
public vpcId: pulumi.Output<string>;
```


The identifier of the VPC in which to create the target group.

<h2 class="pdoc-module-header" id="TargetGroupAttachment">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L12">class TargetGroupAttachment</a>
</h2>

Provides the ability to register instances and containers with an Application Load Balancer (ALB) or Network Load Balancer (NLB) target group. For attaching resources with Elastic Load Balancer (ELB), see the [`aws_elb_attachment` resource](https://www.terraform.io/docs/providers/aws/r/elb_attachment.html).

~> **Note:** `aws_alb_target_group_attachment` is known as `aws_lb_target_group_attachment`. The functionality is identical.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L40">constructor</a>
</h3>

```typescript
new TargetGroupAttachment(name: string, args: TargetGroupAttachmentArgs, opts?: pulumi.CustomResourceOptions)
```


Create a TargetGroupAttachment resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L21">method get</a>
</h3>

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: TargetGroupAttachmentState): TargetGroupAttachment
```


Get an existing TargetGroupAttachment resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L13">method getProvider</a>
</h3>

```typescript
getProvider(moduleMember: string): ProviderResource | undefined
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L85">method isInstance</a>
</h3>

```typescript
static isInstance(obj: any): boolean
```


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L28">property availabilityZone</a>
</h3>

```typescript
public availabilityZone: pulumi.Output<string | undefined>;
```


The Availability Zone where the IP address of the target is to be registered.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L80">property id</a>
</h3>

```typescript
id: Output<ID>;
```


id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L32">property port</a>
</h3>

```typescript
public port: pulumi.Output<number | undefined>;
```


The port on which targets receive traffic.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L36">property targetGroupArn</a>
</h3>

```typescript
public targetGroupArn: pulumi.Output<string>;
```


The ARN of the target group with which to register targets

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L40">property targetId</a>
</h3>

```typescript
public targetId: pulumi.Output<string>;
```


The ID of the target. This is the Instance ID for an instance, or the container ID for an ECS container. If the target type is ip, specify an IP address.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L11">property urn</a>
</h3>

```typescript
urn: Output<URN>;
```


urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

<h2 class="pdoc-module-header" id="getListener">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L16">function getListener</a>
</h2>

```typescript
getListener(args?: GetListenerArgs, opts?: pulumi.InvokeOptions): Promise<GetListenerResult>
```


~> **Note:** `aws_alb_listener` is known as `aws_lb_listener`. The functionality is identical.

Provides information about a Load Balancer Listener.

This data source can prove useful when a module accepts an LB Listener as an
input variable and needs to know the LB it is attached to, or other
information specific to the listener in question.

<h2 class="pdoc-module-header" id="getLoadBalancer">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L16">function getLoadBalancer</a>
</h2>

```typescript
getLoadBalancer(args?: GetLoadBalancerArgs, opts?: pulumi.InvokeOptions): Promise<GetLoadBalancerResult>
```


~> **Note:** `aws_alb` is known as `aws_lb`. The functionality is identical.

Provides information about a Load Balancer.

This data source can prove useful when a module accepts an LB as an input
variable and needs to, for example, determine the security groups associated
with it, etc.

<h2 class="pdoc-module-header" id="getTargetGroup">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L16">function getTargetGroup</a>
</h2>

```typescript
getTargetGroup(args?: GetTargetGroupArgs, opts?: pulumi.InvokeOptions): Promise<GetTargetGroupResult>
```


~> **Note:** `aws_alb_target_group` is known as `aws_lb_target_group`. The functionality is identical.

Provides information about a Load Balancer Target Group.

This data source can prove useful when a module accepts an LB Target Group as an
input variable and needs to know its attributes. It can also be used to get the ARN of
an LB Target Group for use in other resources, given LB Target Group name.

<h2 class="pdoc-module-header" id="GetListenerArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L28">interface GetListenerArgs</a>
</h2>

A collection of arguments for invoking getListener.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L32">property arn</a>
</h3>

```typescript
arn?: string;
```


The arn of the listener. Required if `load_balancer_arn` and `port` is not set.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L36">property loadBalancerArn</a>
</h3>

```typescript
loadBalancerArn?: string;
```


The arn of the load balander. Required if `arn` is not set.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L40">property port</a>
</h3>

```typescript
port?: number;
```


The port of the listener. Required if `arn` is not set.

<h2 class="pdoc-module-header" id="GetListenerResult">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L46">interface GetListenerResult</a>
</h2>

A collection of values returned by getListener.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L47">property arn</a>
</h3>

```typescript
arn: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L48">property certificateArn</a>
</h3>

```typescript
certificateArn: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L49">property defaultActions</a>
</h3>

```typescript
defaultActions: { ... }[];
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L57">property id</a>
</h3>

```typescript
id: string;
```


id is the provider-assigned unique ID for this managed resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L50">property loadBalancerArn</a>
</h3>

```typescript
loadBalancerArn: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L51">property port</a>
</h3>

```typescript
port: number;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L52">property protocol</a>
</h3>

```typescript
protocol: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getListener.ts#L53">property sslPolicy</a>
</h3>

```typescript
sslPolicy: string;
```

<h2 class="pdoc-module-header" id="GetLoadBalancerArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L28">interface GetLoadBalancerArgs</a>
</h2>

A collection of arguments for invoking getLoadBalancer.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L32">property arn</a>
</h3>

```typescript
arn?: string;
```


The full ARN of the load balancer.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L36">property name</a>
</h3>

```typescript
name?: string;
```


The unique name of the load balancer.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L37">property tags</a>
</h3>

```typescript
tags?: { ... };
```

<h2 class="pdoc-module-header" id="GetLoadBalancerResult">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L43">interface GetLoadBalancerResult</a>
</h2>

A collection of values returned by getLoadBalancer.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L44">property accessLogs</a>
</h3>

```typescript
accessLogs: { ... };
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L45">property arn</a>
</h3>

```typescript
arn: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L46">property arnSuffix</a>
</h3>

```typescript
arnSuffix: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L47">property dnsName</a>
</h3>

```typescript
dnsName: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L48">property enableDeletionProtection</a>
</h3>

```typescript
enableDeletionProtection: boolean;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L62">property id</a>
</h3>

```typescript
id: string;
```


id is the provider-assigned unique ID for this managed resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L49">property idleTimeout</a>
</h3>

```typescript
idleTimeout: number;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L50">property internal</a>
</h3>

```typescript
internal: boolean;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L51">property loadBalancerType</a>
</h3>

```typescript
loadBalancerType: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L52">property name</a>
</h3>

```typescript
name: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L53">property securityGroups</a>
</h3>

```typescript
securityGroups: string[];
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L54">property subnetMappings</a>
</h3>

```typescript
subnetMappings: { ... }[];
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L55">property subnets</a>
</h3>

```typescript
subnets: string[];
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L56">property tags</a>
</h3>

```typescript
tags: { ... };
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L57">property vpcId</a>
</h3>

```typescript
vpcId: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getLoadBalancer.ts#L58">property zoneId</a>
</h3>

```typescript
zoneId: string;
```

<h2 class="pdoc-module-header" id="GetTargetGroupArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L28">interface GetTargetGroupArgs</a>
</h2>

A collection of arguments for invoking getTargetGroup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L32">property arn</a>
</h3>

```typescript
arn?: string;
```


The full ARN of the target group.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L36">property name</a>
</h3>

```typescript
name?: string;
```


The unique name of the target group.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L37">property tags</a>
</h3>

```typescript
tags?: { ... };
```

<h2 class="pdoc-module-header" id="GetTargetGroupResult">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L43">interface GetTargetGroupResult</a>
</h2>

A collection of values returned by getTargetGroup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L44">property arn</a>
</h3>

```typescript
arn: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L45">property arnSuffix</a>
</h3>

```typescript
arnSuffix: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L46">property deregistrationDelay</a>
</h3>

```typescript
deregistrationDelay: number;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L47">property healthCheck</a>
</h3>

```typescript
healthCheck: { ... };
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L58">property id</a>
</h3>

```typescript
id: string;
```


id is the provider-assigned unique ID for this managed resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L48">property name</a>
</h3>

```typescript
name: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L49">property port</a>
</h3>

```typescript
port: number;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L50">property protocol</a>
</h3>

```typescript
protocol: string;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L51">property slowStart</a>
</h3>

```typescript
slowStart: number;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L52">property stickiness</a>
</h3>

```typescript
stickiness: { ... };
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L53">property tags</a>
</h3>

```typescript
tags: { ... };
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/getTargetGroup.ts#L54">property vpcId</a>
</h3>

```typescript
vpcId: string;
```

<h2 class="pdoc-module-header" id="ListenerArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L133">interface ListenerArgs</a>
</h2>

The set of arguments for constructing a Listener resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L137">property certificateArn</a>
</h3>

```typescript
certificateArn?: pulumi.Input<string>;
```


The ARN of the default SSL server certificate. Exactly one certificate is required if the protocol is HTTPS. For adding additional SSL certificates, see the [`aws_lb_listener_certificate` resource](https://www.terraform.io/docs/providers/aws/r/lb_listener_certificate.html).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L141">property defaultAction</a>
</h3>

```typescript
defaultAction: pulumi.Input<{ ... }>;
```


An Action block. Action blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L145">property loadBalancerArn</a>
</h3>

```typescript
loadBalancerArn: pulumi.Input<string>;
```


The ARN of the load balancer.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L149">property port</a>
</h3>

```typescript
port: pulumi.Input<number>;
```


The port. Specify a value from `1` to `65535` or `#{port}`. Defaults to `#{port}`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L153">property protocol</a>
</h3>

```typescript
protocol?: pulumi.Input<string>;
```


The protocol. Valid values are `HTTP`, `HTTPS`, or `#{protocol}`. Defaults to `#{protocol}`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L157">property sslPolicy</a>
</h3>

```typescript
sslPolicy?: pulumi.Input<string>;
```


The name of the SSL Policy for the listener. Required if `protocol` is `HTTPS`.

<h2 class="pdoc-module-header" id="ListenerCertificateArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L82">interface ListenerCertificateArgs</a>
</h2>

The set of arguments for constructing a ListenerCertificate resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L86">property certificateArn</a>
</h3>

```typescript
certificateArn: pulumi.Input<string>;
```


The ARN of the certificate to attach to the listener.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L90">property listenerArn</a>
</h3>

```typescript
listenerArn: pulumi.Input<string>;
```


The ARN of the listener to which to attach the certificate.

<h2 class="pdoc-module-header" id="ListenerCertificateState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L68">interface ListenerCertificateState</a>
</h2>

Input properties used for looking up and filtering ListenerCertificate resources.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L72">property certificateArn</a>
</h3>

```typescript
certificateArn?: pulumi.Input<string>;
```


The ARN of the certificate to attach to the listener.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerCertificate.ts#L76">property listenerArn</a>
</h3>

```typescript
listenerArn?: pulumi.Input<string>;
```


The ARN of the listener to which to attach the certificate.

<h2 class="pdoc-module-header" id="ListenerRuleArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L113">interface ListenerRuleArgs</a>
</h2>

The set of arguments for constructing a ListenerRule resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L117">property actions</a>
</h3>

```typescript
actions: pulumi.Input<pulumi.Input<{ ... }>[]>;
```


An Action block. Action blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L121">property conditions</a>
</h3>

```typescript
conditions: pulumi.Input<pulumi.Input<{ ... }>[]>;
```


A Condition block. Condition blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L125">property listenerArn</a>
</h3>

```typescript
listenerArn: pulumi.Input<string>;
```


The ARN of the listener to which to attach the rule.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L129">property priority</a>
</h3>

```typescript
priority?: pulumi.Input<number>;
```


The priority for the rule between `1` and `50000`. Leaving it unset will automatically set the rule with next available priority after currently existing highest rule. A listener can't have multiple rules with the same priority.

<h2 class="pdoc-module-header" id="ListenerRuleState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L87">interface ListenerRuleState</a>
</h2>

Input properties used for looking up and filtering ListenerRule resources.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L91">property actions</a>
</h3>

```typescript
actions?: pulumi.Input<pulumi.Input<{ ... }>[]>;
```


An Action block. Action blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L95">property arn</a>
</h3>

```typescript
arn?: pulumi.Input<string>;
```


The ARN of the rule (matches `id`)

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L99">property conditions</a>
</h3>

```typescript
conditions?: pulumi.Input<pulumi.Input<{ ... }>[]>;
```


A Condition block. Condition blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L103">property listenerArn</a>
</h3>

```typescript
listenerArn?: pulumi.Input<string>;
```


The ARN of the listener to which to attach the rule.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listenerRule.ts#L107">property priority</a>
</h3>

```typescript
priority?: pulumi.Input<number>;
```


The priority for the rule between `1` and `50000`. Leaving it unset will automatically set the rule with next available priority after currently existing highest rule. A listener can't have multiple rules with the same priority.

<h2 class="pdoc-module-header" id="ListenerState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L99">interface ListenerState</a>
</h2>

Input properties used for looking up and filtering Listener resources.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L103">property arn</a>
</h3>

```typescript
arn?: pulumi.Input<string>;
```


The ARN of the listener (matches `id`)

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L107">property certificateArn</a>
</h3>

```typescript
certificateArn?: pulumi.Input<string>;
```


The ARN of the default SSL server certificate. Exactly one certificate is required if the protocol is HTTPS. For adding additional SSL certificates, see the [`aws_lb_listener_certificate` resource](https://www.terraform.io/docs/providers/aws/r/lb_listener_certificate.html).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L111">property defaultAction</a>
</h3>

```typescript
defaultAction?: pulumi.Input<{ ... }>;
```


An Action block. Action blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L115">property loadBalancerArn</a>
</h3>

```typescript
loadBalancerArn?: pulumi.Input<string>;
```


The ARN of the load balancer.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L119">property port</a>
</h3>

```typescript
port?: pulumi.Input<number>;
```


The port. Specify a value from `1` to `65535` or `#{port}`. Defaults to `#{port}`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L123">property protocol</a>
</h3>

```typescript
protocol?: pulumi.Input<string>;
```


The protocol. Valid values are `HTTP`, `HTTPS`, or `#{protocol}`. Defaults to `#{protocol}`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/listener.ts#L127">property sslPolicy</a>
</h3>

```typescript
sslPolicy?: pulumi.Input<string>;
```


The name of the SSL Policy for the listener. Required if `protocol` is `HTTPS`.

<h2 class="pdoc-module-header" id="LoadBalancerArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L250">interface LoadBalancerArgs</a>
</h2>

The set of arguments for constructing a LoadBalancer resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L254">property accessLogs</a>
</h3>

```typescript
accessLogs?: pulumi.Input<{ ... }>;
```


An Access Logs block. Access Logs documented below. Only valid for Load Balancers of type `application`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L259">property enableCrossZoneLoadBalancing</a>
</h3>

```typescript
enableCrossZoneLoadBalancing?: pulumi.Input<boolean>;
```


If true, cross-zone load balancing of the load balancer will be enabled.
This is a `network` load balancer feature. Defaults to `false`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L264">property enableDeletionProtection</a>
</h3>

```typescript
enableDeletionProtection?: pulumi.Input<boolean>;
```


If true, deletion of the load balancer will be disabled via
the AWS API. This will prevent Terraform from deleting the load balancer. Defaults to `false`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L268">property enableHttp2</a>
</h3>

```typescript
enableHttp2?: pulumi.Input<boolean>;
```


Indicates whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L272">property idleTimeout</a>
</h3>

```typescript
idleTimeout?: pulumi.Input<number>;
```


The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L276">property internal</a>
</h3>

```typescript
internal?: pulumi.Input<boolean>;
```


If true, the LB will be internal.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L280">property ipAddressType</a>
</h3>

```typescript
ipAddressType?: pulumi.Input<string>;
```


The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L284">property loadBalancerType</a>
</h3>

```typescript
loadBalancerType?: pulumi.Input<string>;
```


The type of load balancer to create. Possible values are `application` or `network`. The default value is `application`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L290">property name</a>
</h3>

```typescript
name?: pulumi.Input<string>;
```


The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
Terraform will autogenerate a name beginning with `tf-lb`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L294">property namePrefix</a>
</h3>

```typescript
namePrefix?: pulumi.Input<string>;
```


Creates a unique name beginning with the specified prefix. Conflicts with `name`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L298">property securityGroups</a>
</h3>

```typescript
securityGroups?: pulumi.Input<pulumi.Input<string>[]>;
```


A list of security group IDs to assign to the LB. Only valid for Load Balancers of type `application`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L302">property subnetMappings</a>
</h3>

```typescript
subnetMappings?: pulumi.Input<pulumi.Input<{ ... }>[]>;
```


A subnet mapping block as documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L308">property subnets</a>
</h3>

```typescript
subnets?: pulumi.Input<pulumi.Input<string>[]>;
```


A list of subnet IDs to attach to the LB. Subnets
cannot be updated for Load Balancers of type `network`. Changing this value
for load balancers of type `network` will force a recreation of the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L312">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```


A mapping of tags to assign to the resource.

<h2 class="pdoc-module-header" id="LoadBalancerState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L165">interface LoadBalancerState</a>
</h2>

Input properties used for looking up and filtering LoadBalancer resources.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L169">property accessLogs</a>
</h3>

```typescript
accessLogs?: pulumi.Input<{ ... }>;
```


An Access Logs block. Access Logs documented below. Only valid for Load Balancers of type `application`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L173">property arn</a>
</h3>

```typescript
arn?: pulumi.Input<string>;
```


The ARN of the load balancer (matches `id`).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L177">property arnSuffix</a>
</h3>

```typescript
arnSuffix?: pulumi.Input<string>;
```


The ARN suffix for use with CloudWatch Metrics.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L181">property dnsName</a>
</h3>

```typescript
dnsName?: pulumi.Input<string>;
```


The DNS name of the load balancer.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L186">property enableCrossZoneLoadBalancing</a>
</h3>

```typescript
enableCrossZoneLoadBalancing?: pulumi.Input<boolean>;
```


If true, cross-zone load balancing of the load balancer will be enabled.
This is a `network` load balancer feature. Defaults to `false`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L191">property enableDeletionProtection</a>
</h3>

```typescript
enableDeletionProtection?: pulumi.Input<boolean>;
```


If true, deletion of the load balancer will be disabled via
the AWS API. This will prevent Terraform from deleting the load balancer. Defaults to `false`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L195">property enableHttp2</a>
</h3>

```typescript
enableHttp2?: pulumi.Input<boolean>;
```


Indicates whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L199">property idleTimeout</a>
</h3>

```typescript
idleTimeout?: pulumi.Input<number>;
```


The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L203">property internal</a>
</h3>

```typescript
internal?: pulumi.Input<boolean>;
```


If true, the LB will be internal.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L207">property ipAddressType</a>
</h3>

```typescript
ipAddressType?: pulumi.Input<string>;
```


The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L211">property loadBalancerType</a>
</h3>

```typescript
loadBalancerType?: pulumi.Input<string>;
```


The type of load balancer to create. Possible values are `application` or `network`. The default value is `application`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L217">property name</a>
</h3>

```typescript
name?: pulumi.Input<string>;
```


The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
Terraform will autogenerate a name beginning with `tf-lb`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L221">property namePrefix</a>
</h3>

```typescript
namePrefix?: pulumi.Input<string>;
```


Creates a unique name beginning with the specified prefix. Conflicts with `name`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L225">property securityGroups</a>
</h3>

```typescript
securityGroups?: pulumi.Input<pulumi.Input<string>[]>;
```


A list of security group IDs to assign to the LB. Only valid for Load Balancers of type `application`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L229">property subnetMappings</a>
</h3>

```typescript
subnetMappings?: pulumi.Input<pulumi.Input<{ ... }>[]>;
```


A subnet mapping block as documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L235">property subnets</a>
</h3>

```typescript
subnets?: pulumi.Input<pulumi.Input<string>[]>;
```


A list of subnet IDs to attach to the LB. Subnets
cannot be updated for Load Balancers of type `network`. Changing this value
for load balancers of type `network` will force a recreation of the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L239">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```


A mapping of tags to assign to the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L240">property vpcId</a>
</h3>

```typescript
vpcId?: pulumi.Input<string>;
```

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/loadBalancer.ts#L244">property zoneId</a>
</h3>

```typescript
zoneId?: pulumi.Input<string>;
```


The canonical hosted zone ID of the load balancer (to be used in a Route 53 Alias record).

<h2 class="pdoc-module-header" id="TargetGroupArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L213">interface TargetGroupArgs</a>
</h2>

The set of arguments for constructing a TargetGroup resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L217">property deregistrationDelay</a>
</h3>

```typescript
deregistrationDelay?: pulumi.Input<number>;
```


The amount time for Elastic Load Balancing to wait before changing the state of a deregistering target from draining to unused. The range is 0-3600 seconds. The default value is 300 seconds.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L221">property healthCheck</a>
</h3>

```typescript
healthCheck?: pulumi.Input<{ ... }>;
```


A Health Check block. Health Check blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L225">property name</a>
</h3>

```typescript
name?: pulumi.Input<string>;
```


The name of the target group. If omitted, Terraform will assign a random, unique name.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L229">property namePrefix</a>
</h3>

```typescript
namePrefix?: pulumi.Input<string>;
```


Creates a unique name beginning with the specified prefix. Conflicts with `name`. Cannot be longer than 6 characters.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L233">property port</a>
</h3>

```typescript
port: pulumi.Input<number>;
```


The port to use to connect with the target. Valid values are either ports 1-65536, or `traffic-port`. Defaults to `traffic-port`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L237">property protocol</a>
</h3>

```typescript
protocol: pulumi.Input<string>;
```


The protocol to use to connect with the target. Defaults to `HTTP`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L241">property proxyProtocolV2</a>
</h3>

```typescript
proxyProtocolV2?: pulumi.Input<boolean>;
```


Boolean to enable / disable support for proxy protocol v2 on Network Load Balancers. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/load-balancer-target-groups.html#proxy-protocol) for more information.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L245">property slowStart</a>
</h3>

```typescript
slowStart?: pulumi.Input<number>;
```


The amount time for targets to warm up before the load balancer sends them a full share of requests. The range is 30-900 seconds or 0 to disable. The default value is 0 seconds.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L249">property stickiness</a>
</h3>

```typescript
stickiness?: pulumi.Input<{ ... }>;
```


A Stickiness block. Stickiness blocks are documented below. `stickiness` is only valid if used with Load Balancers of type `Application`

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L253">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```


A mapping of tags to assign to the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L262">property targetType</a>
</h3>

```typescript
targetType?: pulumi.Input<string>;
```


The type of target that you must specify when registering targets with this target group.
The possible values are `instance` (targets are specified by instance ID) or `ip` (targets are specified by IP address).
The default is `instance`. Note that you can't specify targets for a target group using both instance IDs and IP addresses.
If the target type is `ip`, specify IP addresses from the subnets of the virtual private cloud (VPC) for the target group,
the RFC 1918 range (10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16), and the RFC 6598 range (100.64.0.0/10).
You can't specify publicly routable IP addresses.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L266">property vpcId</a>
</h3>

```typescript
vpcId: pulumi.Input<string>;
```


The identifier of the VPC in which to create the target group.

<h2 class="pdoc-module-header" id="TargetGroupAttachmentArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L100">interface TargetGroupAttachmentArgs</a>
</h2>

The set of arguments for constructing a TargetGroupAttachment resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L104">property availabilityZone</a>
</h3>

```typescript
availabilityZone?: pulumi.Input<string>;
```


The Availability Zone where the IP address of the target is to be registered.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L108">property port</a>
</h3>

```typescript
port?: pulumi.Input<number>;
```


The port on which targets receive traffic.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L112">property targetGroupArn</a>
</h3>

```typescript
targetGroupArn: pulumi.Input<string>;
```


The ARN of the target group with which to register targets

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L116">property targetId</a>
</h3>

```typescript
targetId: pulumi.Input<string>;
```


The ID of the target. This is the Instance ID for an instance, or the container ID for an ECS container. If the target type is ip, specify an IP address.

<h2 class="pdoc-module-header" id="TargetGroupAttachmentState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L78">interface TargetGroupAttachmentState</a>
</h2>

Input properties used for looking up and filtering TargetGroupAttachment resources.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L82">property availabilityZone</a>
</h3>

```typescript
availabilityZone?: pulumi.Input<string>;
```


The Availability Zone where the IP address of the target is to be registered.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L86">property port</a>
</h3>

```typescript
port?: pulumi.Input<number>;
```


The port on which targets receive traffic.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L90">property targetGroupArn</a>
</h3>

```typescript
targetGroupArn?: pulumi.Input<string>;
```


The ARN of the target group with which to register targets

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroupAttachment.ts#L94">property targetId</a>
</h3>

```typescript
targetId?: pulumi.Input<string>;
```


The ID of the target. This is the Instance ID for an instance, or the container ID for an ECS container. If the target type is ip, specify an IP address.

<h2 class="pdoc-module-header" id="TargetGroupState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L146">interface TargetGroupState</a>
</h2>

Input properties used for looking up and filtering TargetGroup resources.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L150">property arn</a>
</h3>

```typescript
arn?: pulumi.Input<string>;
```


The ARN of the Target Group (matches `id`)

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L154">property arnSuffix</a>
</h3>

```typescript
arnSuffix?: pulumi.Input<string>;
```


The ARN suffix for use with CloudWatch Metrics.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L158">property deregistrationDelay</a>
</h3>

```typescript
deregistrationDelay?: pulumi.Input<number>;
```


The amount time for Elastic Load Balancing to wait before changing the state of a deregistering target from draining to unused. The range is 0-3600 seconds. The default value is 300 seconds.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L162">property healthCheck</a>
</h3>

```typescript
healthCheck?: pulumi.Input<{ ... }>;
```


A Health Check block. Health Check blocks are documented below.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L166">property name</a>
</h3>

```typescript
name?: pulumi.Input<string>;
```


The name of the target group. If omitted, Terraform will assign a random, unique name.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L170">property namePrefix</a>
</h3>

```typescript
namePrefix?: pulumi.Input<string>;
```


Creates a unique name beginning with the specified prefix. Conflicts with `name`. Cannot be longer than 6 characters.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L174">property port</a>
</h3>

```typescript
port?: pulumi.Input<number>;
```


The port to use to connect with the target. Valid values are either ports 1-65536, or `traffic-port`. Defaults to `traffic-port`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L178">property protocol</a>
</h3>

```typescript
protocol?: pulumi.Input<string>;
```


The protocol to use to connect with the target. Defaults to `HTTP`.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L182">property proxyProtocolV2</a>
</h3>

```typescript
proxyProtocolV2?: pulumi.Input<boolean>;
```


Boolean to enable / disable support for proxy protocol v2 on Network Load Balancers. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/load-balancer-target-groups.html#proxy-protocol) for more information.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L186">property slowStart</a>
</h3>

```typescript
slowStart?: pulumi.Input<number>;
```


The amount time for targets to warm up before the load balancer sends them a full share of requests. The range is 30-900 seconds or 0 to disable. The default value is 0 seconds.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L190">property stickiness</a>
</h3>

```typescript
stickiness?: pulumi.Input<{ ... }>;
```


A Stickiness block. Stickiness blocks are documented below. `stickiness` is only valid if used with Load Balancers of type `Application`

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L194">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```


A mapping of tags to assign to the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L203">property targetType</a>
</h3>

```typescript
targetType?: pulumi.Input<string>;
```


The type of target that you must specify when registering targets with this target group.
The possible values are `instance` (targets are specified by instance ID) or `ip` (targets are specified by IP address).
The default is `instance`. Note that you can't specify targets for a target group using both instance IDs and IP addresses.
If the target type is `ip`, specify IP addresses from the subnets of the virtual private cloud (VPC) for the target group,
the RFC 1918 range (10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16), and the RFC 6598 range (100.64.0.0/10).
You can't specify publicly routable IP addresses.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/applicationloadbalancing/targetGroup.ts#L207">property vpcId</a>
</h3>

```typescript
vpcId?: pulumi.Input<string>;
```


The identifier of the VPC in which to create the target group.

