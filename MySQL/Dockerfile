FROM mysql:8.0

LABEL maintainer="xiaoyi"

ARG start_type

#####################################
# Set Timezone
#####################################
RUN echo ${start_type}

COPY ./${start_type}/my.cnf /etc/mysql/conf.d/my.cnf

RUN chmod 0444 /etc/mysql/conf.d/my.cnf

CMD ["mysqld"]

EXPOSE 3306