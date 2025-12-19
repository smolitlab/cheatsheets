# Sveltos Cheat Sheet

## Kubectl commands to check sveltos CRDs

Get clusters managed by Sveltos
    
    kubectl get sveltosclusters -A
 
    kubectl get sveltosclusters -A --show-labels
 
ClusterSummary        Shows the status of applied ClusterProfiles
    
    kubectl get clustersummary -A

ClusterProfile  Defines add-ons and policies applied to clusters

    kubectl get clusterprofiles -A
 

Classifier        Groups clusters based on labels or conditions

    kubectl get classifiers -A
 
EventSource  Watches cluster events for automation

    kubectl get eventsource -A


## Sceltosctl commands

Addon Represents a Helm chart or manifest deployed to clusters

    sveltosctl show addons
 
Display information about resources in managed clusters.

    sveltosctl show resources
 

Displays information:

- Which clusters are currently a match for a ClusterProfile;

- For ConfigMap/Secret list of clusters where their content is currently deployed.

        sveltosctl show usage

Sources:

https://projectsveltos.github.io/sveltos/main/getting_started/sveltosctl/features/visibility/