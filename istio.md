### virtual Service
Configuration affecting traffic routing.

Service a unit of application behavior bound to a unique name in a service registry. Services consist of multiple network endpoints implemented by workload instances running on pods, containers, VMs etc.

Source - A downstream client calling a service.

Host - The address used by a client when attempting to connect to a service.

Destination indicates the network addressable service to which the request/connection will be sent after processing a routing rule. 
The destination, host should unambiguously refer to a service in the service registry. Istio's service registry is composed of all the services found in the platform's service registry, as well as services declared through the ServiceEntry resource.




### destination rule
DestinationRule defines policies that apply to traffic intended for a service after routing has occurred. These rules specify configuration for load balancing, connection pool size from the sidecar.
