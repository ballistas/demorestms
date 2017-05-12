FROM openjdk:8-jdk
MAINTAINER Patrick Kunert <patrick.kunert@gmail.com>

ENTRYPOINT ["/usr/bin/java", "-jar", "/usr/share/payment/demo/demoservice.jar"]

# Add Maven dependencies (not shaded into the artifact; Docker-cached)
#ADD target/lib /usr/share/payment/demo/lib
# Add the service itself
ADD demo-rest-ms-1.0-SNAPSHOT.jar /usr/share/payment/demo/demoservice.jar