# N8N Automation

[![Product Name Screen Shot][product-screenshot]](https://example.com)

This project is for <h1>JERUSALEM POST LTD</h1> Company automation.

This includes various n8n flows such as <b>Radio news</b>, <b>Groq traslation</b>, <b>Groq transcript</b>,
<b>Mistral OCR</b>, <b>Google OCR</b>, <b>Create News Narration</b>.

### Requirements

- n8n environment
- Credentials such as Groq, Google Service Account, Google Storage Credential

### Project Structure

- [N8N Automation](#n8n-automation)
  - [Requirements](#requirements)
  - [Project Structure](#project-structure)
  - [Credential](#credential)
  - [Flow](#flow)
    - [Radio News](#radio-news)
    - [Mistral OCR](#mistral-ocr)
    - [Google OCR](#google-ocr)
    - [Groq Translate](#groq-translate)
    - [Groq Transcript](#groq-transcript)
    - [Generate Video](#generate-video)

### Credential

- Groq

  ```sh
  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
  ```

- Google Service Account

  ```sh
  type: service_account,
  ```

  ```sh
  project_id: radiant-mason-455819-q6
  ```

  ```sh
  private_key_id: 613b012bba56b02c07bd0f39e9c3df0d4ea86fd8
  ```

  ```sh
  private_key: -----BEGIN PRIVATE KEY-----\nMIIEvgIBADANBgkqhkiG9w0BAQEFAASCBKgwggSkAgEAAoIBAQCUtS8J8T/TwbAR\n2dBeRAGLEvrKpMgVF8QU5S1OmNYQkdx4YtAAFsaA5blQe7o6jUbEPNClGbxZ4pX2\ncHukWA4dTYMiwUMjJUCwn/nRw0sgmJHbSsG5oeLqT73onTEPUZykIJ+SIyoWGRNm\nuA3K9MYL9kjfgY6T/eKprmEXp36mzIeot4ILAMDJg5WqUA3BWez8lx+oV/u2za6d\ncxQO2ow3Pb+WGNmY8VqsgXk/hTljUvF5a11QM03KY6qQ4k88D9TAOquEiMl4DvnR\nATpByzJ37t34YCDygmxzJHhSyqlEGw2C20iS+nibr841rrq+T+BXwkUlMldEcwiT\n6U8ATPJDAgMBAAECggEAMKb0jFKvOLciRTzXdLfYL2mWvqzZvzjm0JVIVPIg+wvV\nr1dYyOaqrCo8jm3keFqXYAWrl5CLdHby7E1Rzmt2trSQ5lKHhhyehQrZ33x+/Fue\nQLo9FmA2DsXnEo83KVVgo7v+qP+zOcabd9xYuuGJWAmMPv+yp42FVlF0d5o3kBdT\nuLfHxOvr+deRzO4VJKQ73VbSZEBJ0pr1q7Fs+mh9AMEAz2NAYHqPZ93M1wok9XJI\nH71Jm5xMrAmCpJkhkH7jSkGSAUZ68ZTSvofbxMPHijQs8sm98YehF5MVtcM2ZneL\n73sL78j+ek6DyQPp4B5fFgGE3HFbGIaMlZgKFndcKQKBgQDKzkRmPnKyXuxIofDi\nBSiL2Zu9FPmHBo5yh/cDSZ2hssOvNG2qn8TZLZmox+CLtDFCVvDuMLARdmiGslg/\n2mEpzqjANx5aHtIPr7kVeAbXwJONoUqoROSDe0vB9Copvj695N+I8nvvupSa54dh\nBv9T0hF3rEhdPxXWyRtED5KaGQKBgQC7tmqT96Lcr3OKXye3ldnMJKnINBiLHK8O\ncYln44RPJXftEmVYrlynMglr5Ce/+WqCDpaSPP+NTCcLm2T66nMM8/WleGdq6Y8a\nGTo3/cZVKiJXxd4tTp0YwOAIqgma8hkyjNgxnXBII9R840mEO2v+y9oE7PT9hs9a\nNKD5nbmyuwKBgQC31IKhnyd+UZaiO9BKP9zB741Atlt8rk++t0oLO9ZbtNu127Mw\nf0QCjFgFarA6Uip4dLBNZ+qg2ZDjz5M4xe1e5QmHui6UB+3m9CSztimVteTJ85Ll\nthTgrYk9FOKHFgBvRp/s1cfLxHdhdk77f0k/pGHa9Vpe04krOP2zEt6TOQKBgFBK\nNkwUIBVE9qa5DMP51K78/6IiplzaaAZFigBl0LIJ1MISnEbSTc82F9GORXJXvLbk\nhoMGlEhbylesoASzQ4LG1stwNMwGGq+PGtfYNH05CHeCqwW2Gnv8A9ew42rjIuP8\nWnzeWqiAquLAVTG6OPdDOn3g3OmUQBzVZgVe8Y8BAoGBAIFbU9aF6C40RXzk7VOa\nHRT9BgzjJIHkT0LUXPFsDexhYgGAU0iYuaxhVem+bT+fjjKB5kUDE1NO3A+CCvy5\nfc/zanDO+hGlmX6rVIGtVpTaLYn//45yfCfy7iLx+c8gvBHd+GmW6pqzMUJqJVut\nLnhdA8aAurXP8O4P3yqK1qC0\n-----END PRIVATE KEY-----\n
  ```

  ```sh
  client_email: ocr-service-account@radiant-mason-455819-q6.iam.gserviceaccount.com
  ```

  ```sh
  client_id : 117922853670374624280
  ```

  ```sh
  auth_uri : https://accounts.google.com/o/oauth2/auth
  ```

  ```sh
  token_uri : https://oauth2.googleapis.com/token
  ```

  ```sh
  auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs
  ```

  ```sh
  client_x509_cert_url : https://www.googleapis.com/robot/v1/metadata/x509/ocr-service-account%40radiant-mason-455819-q6.iam.gserviceaccount.com

  ```

  ```sh
  universe_domain: googleapis.com
  ```

- ShotStack
  ```sh
  Sandbox(jag2pn7hng) : T0mZ85JFMS87u5WYArIGSwQymiCArn511BWJjCjg
  Production(Mz1eil9p3p) : 1GSC6MeVhQ2FClIfvCKqS4NA8TRVwr91M0VBT1qf
  ```

### Flow

#### Radio News

Send radio news every 15 minutes except Friday, Saturday.

#### Mistral OCR

Extract text from images and PDF using Mistral OCR.

#### Google OCR

Extract text from images and PDF using Google OCR.

#### Groq Translate

Translate text using Groq Translate.

#### Groq Transcript

Transcriipt audio using Groq Transcript.

#### Generate Video

Generate video using ShotStack SDK.

[product-screenshot]: https://user-images.githubusercontent.com/10284570/173569848-c624317f-42b1-45a6-ab09-f0ea3c247648.png
