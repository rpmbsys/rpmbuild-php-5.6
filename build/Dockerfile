ARG rocky=8.10.20240528
FROM aursu/rpmbuild:${rocky}-build

USER root

COPY system/etc/yum.repos.d/bintray-custom-rocky.repo /etc/yum.repos.d/bintray-custom.repo

RUN dnf -y --enablerepo=bintray-custom --enablerepo=bintray-phpcustom install \
        php-cli-5.6.40 \
        php-common-5.6.40 \
        php-devel-5.6.40 \
        php-process-5.6.40 \
        php-xml-5.6.40 \
    && dnf clean all && rm -rf /var/cache/dnf /var/lib/rpm/__db*
