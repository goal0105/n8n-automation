# N8N Automation

This project is for JERUSALEM POST LTD Company automation.

This includes various n8n flows such as radio news, Groq traslation, Groq transcript,
Mistral OCR, Google OCR, Create News Narration.

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

```
  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
```

- Google Service Account :

```
type: service_account,
```

```
project_id: radiant-mason-455819-q6
```

```
private_key_id: 613b012bba56b02c07bd0f39e9c3df0d4ea86fd8
```

```
private_key: -----BEGIN PRIVATE KEY-----\nMIIEvgIBADANBgkqhkiG9w0BAQEFAASCBKgwggSkAgEAAoIBAQCxG37rnQICgTR1\n8qjB1gpoblxHRgaNJ3yRyMTZ3MLQxl681RI9SCGGfq9X/ CEGLxgokH7FAl2gMx+w\nzpmYOzm8/AavVzbvDdUyDQc/yGKs7UFHVXiCX7YWhX9tD6mQPTesYR4oseF2pYaG\n9+6g/ONTBbZPTXQpnwGSwpgcBnYmaweCXACmDm01jD0b736qpS9PXlqfpInTMQSy\nJfymy51qI5/bmOFDpBSNPCaWrPdz4qQTtRE9/H5wT+1NprQSMXBFq6vk6YdZ+ZR2\nxoHS1ukZSpXkFra4fSTcQlqfhIAaJ0qVPSOIVNFBbYCBF37CeY1XKAGhltViQAUt\na80icF7zAgMBAAECggEABU3rA7iB8RGYliMXPdL2IIGUVEglyxV7LCHvZLexbVpQ\n8maOnh+VGCJJiHY926G5H1c7N2r7jeA/cJFc1UvfeKhdtOOvpVeXN+FfAwsyirZX\nuwC1fsYfaIDwEOlOrUoVavLFBKKrO4f38FPoUDxdZ0T9BwFYBiUZLCGVjQVT2uZT\nNAn/UxZBEDeqH8171GgReRDY4nSFEdfpq0Xt5pgPYy+7wKwATPWOw7DTon+mUpL+\n8V5sRvlHcOFpJvklIwuYf9+my+/TUmpP7nE5L3VeclhG74IZ2f5weizcZGirdwwq\nq9ZSuh08cC+53y3ZlFisxUxXodxC4dB63lDHg3I1qQKBgQDx1wLHjLZWc3uvsOXo\nvxuYLMjYK51xoHl0QZ3jhlA2n4O3DFL6SuC7XxQ5gyXy2bCUU9hGooniEzRKIv/l\n9LhTDjHVdE/fOy/kMfhlGS+USrGShbhd9m2O51T69i6Ea0hV5b/BOD8JI7GFNQwh\n6okjSHLVnZcCRvnYllAtPHZ26wKBgQC7ejIzXwB30ZlM8xlIz3zpWYmgMaH9vWzJ\nTULMemoOvr2GBquHEm56g77ZXJIxSWZnFfWpXNZEAKgqJga3qEzwKMiXY+PE01eL\nWO92WJbul5hNf8CS9UeKkr1CoPV8bSnmL6zfIvEJ8l5lIGOEYThqJd1qrfSOCY3y\n1tgWYW/GGQKBgQCA9mthBkRlrYeTlP3FM8P/TkJ8JCX9ZdneiO8tWX6E4mNWxZeq\nKSvWP0mFsc4WxsdHEb8PS7XDfQIxVqCne+yfPb6NWU0OeX18brlLEDczGPHAdNZw\nJO0fe3Txrz33F06nn7C11MyojwQnSLaDj5I54nR6PWM9r6OkP+PZe5igqQKBgQCF\nFRcxtEymwZjrMN5P+0oWc8LofpMZhjAFLd0vPe6vjOMIkw+MEJ9wRLljnv0AE7Sn\nlMUQdqB7IWQ+l0PJd6U2Dh1mqjfzbnsEphtGjViHAgHRcdCIAanJSqUi+ROKQguu\nJUW4GBu3Dd/INZevTzw2za5Bnj6t3UZwjeZS7NPlcQKBgA3Wu9+woKxDfU9l6vEL\n8Tem+G+0rnzpP7YIft6HuvgKEBjiUViSgdmfHP0XtzjZb/AaIggk4PGGhMXV7N8V\nRScdVMfUPLhQtwXx/ KSym2U6IRLrfs78YG198oEofH12AL9qfWYI62Uu6g76i1aK\nHIVdvjIll2eVo4LUAdyoPQ3g\n-----END PRIVATE KEY-----\n
```

```
client_email: ocr-service-account@radiant-mason-455819-q6.iam.gserviceaccount.com
```

```
client_id : 117922853670374624280
```

```
auth_uri : https://accounts.google.com/o/oauth2/auth
```

```
token_uri : https://oauth2.googleapis.com/token
```

```
auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs
```

```
client_x509_cert_url : https://www.googleapis.com/robot/v1/metadata/x509/ocr-service-account%40radiant-mason-455819-q6.iam.gserviceaccount.com

```

```
universe_domain: googleapis.com
```

- ShotStack

```
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
