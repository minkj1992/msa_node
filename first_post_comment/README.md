# simple post and comment msa

- node, express
- react, cra
- skaffold, k8s, docker

## Lessons and Cons

### Lessons

1. Event based Async communication between services
2. Async communication encourages each service to be 100% self-sufficient, which makes easy to handle temp downtime or scale-out or new service creation.
3. Skaffold makes easy to building, pushing and deploying k8s containers infra.

### Cons
1. Lots of duplicated code.
2. Hard to picture flow of events between services -> Airflow + Kafka
3. Hard to test event flows
4. Needs to handle series of events (ordering events, group of events)
5. next time: Skaffold + Kustomize, 
