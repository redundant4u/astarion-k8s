FROM eclipse-temurin:17-jre-alpine

WORKDIR /home/astarion

RUN ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime

COPY data/dependencies .
COPY data/spring-boot-loader .
COPY data/snapshot-dependencies .
COPY data/application .

ENTRYPOINT [ \
    "java", \
    "-Dspring.profiles.active=deploy", \
    "-Duser.timezone=Asia/Seoul", \
    "org.springframework.boot.loader.launch.JarLauncher" \
]
