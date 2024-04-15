# FROM khalosa/rasa-aarch64:3.5.2
FROM rasa/rasa:3.6.19

COPY . /app

WORKDIR /app
USER root
RUN pip install python-dotenv rasa-sdk requests
USER 1001
EXPOSE 5055

CMD ["run", "actions", "--debug"]