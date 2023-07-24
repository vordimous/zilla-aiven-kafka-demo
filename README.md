# zilla-aiven-kafka-demo

- Aiven Kafka
- Zilla SSE
- Vue frontend

Stream raw data to the UI on screen. Poll OS api endpoints to push any random data going through Kafka.

Aiven connection: https://docs.aklivity.io/zilla/latest/guides/connecting-to-kafka/aiven.html#zilla-yaml
basic SSE setup: https://docs.aklivity.io/zilla/latest/get-started/quickstart/sse.html#hello-world-with-sse
zilla-kafka-devrel-ben.aivencloud.com:15545

openssl pkcs12 -export -in service.cert -inkey service.key \
    -out keystore.p12 -name "Aiven_CA_Cert" \
    -CAfile ca.pem

keytool -import -file ca.pem \
    -alias "Aiven_Client_Cert" \
    -keystore truststore.p12

AivenZilla

* alerts and kibana
* Zilla is for real time user value
  * two panels, full stream and a list of the hashes
  * select the hashes to change the stream data
  * zilla publishes the search object onto a topic
  * 
