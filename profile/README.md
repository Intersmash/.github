## Hi there! 👋

🙋‍♀️ **... and welcome to the Intersmash organization!**

[Intersmash](https://github.com/Intersmash) was created by the Red Hat JBoss EAP Software Quality Engineering team, and is made of the following 3 repositories:
- [A set of Java applications](https://github.com/Intersmash/intersmash-applications/tree/main), e.g.: WildFly applications, wihch can be run by application servers 
- [A framewok/library](https://github.com/Intersmash/intersmash/tree/main) that helps developers and testers to build complex scenarios, and test middleware services interoperability in Cloud environments.
- [A bunch of tests](https://github.com/Intersmash/intersmash-tests/tree/main), which can be executed continuosly to validate application requirements and specifics 

The idea is to have a common org where developers and testers can place their Java applications, and implement complex tests that validate how such applications interact with other middleware services on cloud based environments, most notably OpenSHift.


🌈 **How to get involved?**

- Submit a PR to create a Java/Jakarta application, see for example
[Intersmash Applications - WildFly MicroProfile Reactive Messaging + Kafka](https://github.com/Intersmash/intersmash-applications/tree/main/wildfly/microprofile-reactive-messaging-kafka#intersmash-applications---wildfly-microprofile-reactive-messaging--kafka)
to the [intersmash-applications repository](https://github.com/Intersmash/intersmash-applications/tree/main)
- Read the [Intermash framework documentation](https://github.com/Intersmash/intersmash/blob/main/docs/GETTING_STARTED.md#getting-started), 
and see how to create one or more _application descriptors_ (i.e. Java classes) that represent a given service you want to be provisioned on the target Cloud environment 
- Create an integration test, which is expected to validate the application behavior on OpenShift, specifically with respect to the interaction with other Middleware services, as for instance Keycloak, or Kafka.
See for instance the [WildFly MicroProfile Reactive Messaging + Kafka](https://github.com/fabiobrz/intersmash-tests/tree/main/wildfly-microprofile-reactive-messaging-kafka#intersmash-tests---wildfly-microprofile-reactive-messaging--kafka)

That's it! Once reviewed, the Intersmash maintainers will run the CI e2e workflow that will validate the application and the test, which will be merged once a green bar is reported.
After that, your test will be part of the [intersmash-tests](https://github.com/fabiobrz/intersmash-tests/tree/main) codebase, which can be used to keep the Middleware services interoperability cloud scenarios under control, continuosly 🙂 


👩‍💻 **Useful resources**

- [Kubernetes](https://kubernetes.io/)
- [OpenShift](https://www.redhat.com/en/technologies/cloud-computing/openshift)
- [CodeReady Containers (CRC)](https://github.com/crc-org/crc): a single node OpenShift cluster implementation that can be run locally
- [Intersmash framweork documentation](https://github.com/Intersmash/intersmash/blob/main/README.md)


🍿 **Fun facts, and some history**

Intersmash was initially an internal project, named "Appsint", by a small team of Red Hat JBoss QEs, and it was implemented as a single repository, containing both the tools, applications and tests.
It was used to test JBoss EAP 7.3 and 7.4 interoperability with other Red Hat products, as:
- Red Hat Datagrid
- Red Hat SSO (now Red Hat Build of Keycloak) 
- Red Hat AMQ Broker
- Red Hat AMQ Streams (now Streams for Apache Kafka)

After some time we decided to split the repo, and separated the framework and core components from the applications and tests.
This scaled better, but we needed  little bit more help to implement provisioning tooling for more services, so we decided to bring the framework to the community, and created the [Intersmash repository](https://github.com/Intersmash/intersmash).
This way we could test JBoss EAP 8 Beta, JBoss EAP XP 5, and now JBoss EAP.1 Beta and JBoss EAP XP 6 interoperability scenarios on OpenShift.
Tests are still being stored in internal Red Hat repositorie, and executed by internal continuous testing pipelines.

Lately we started an effort to bring applications and tests upstream as well, in order to be able to test both commuity bits and deliverables and their product variants, 
within a common upstream org to foster collaboration between people working on one or more services.

Yes, we know, there is _a lot_ which can be improved here 🙂... And we do welcome any contributions!
Feel free to reach out, submit an issue or a PR to improve the code or to create a new test.
It will all contribute to make Middleware services quality better!

Cheers!

<!--
https://github.com/Intersmash/intersmash
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
