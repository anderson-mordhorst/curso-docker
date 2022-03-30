FROM python:3.6
LABEL maintainer 'Aluno Cod3r <aluno at cod3r.com.br>'

# Cada run gera uma layer na imagem
RUN useradd www && \
    mkdir /app && \
    mkdir /log && \
    chown www /log

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000

# Processo que será executado ao subir o container
ENTRYPOINT ["/usr/local/bin/python"]
# Não precisa copiar esse aquivo pra dentro da imagem?
CMD ["run.py"]