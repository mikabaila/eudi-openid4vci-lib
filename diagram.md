''' mermaid
classDiagram
    class Issuer {
        +CredentialOffer credentialOffer
        +DPoPJwtFactory dPoPJwtFactory
        +DeferredIssuanceContext deferredContext(deferredCredential: SubmissionOutcome.Deferred)
    }
    class AuthorizeIssuance
    class RequestIssuance
    class QueryForDeferredCredential
    class NotifyIssuer
    class CredentialOffer
    class DPoPJwtFactory
    class DeferredIssuanceContext
    class SubmissionOutcome {
        class Deferred
    }
    class OpenId4VCIConfig
    class HttpClient
    class CredentialIssuerId
    class CredentialIssuerMetadata
    class CIAuthorizationServerMetadata
    class KtorHttpClientFactory
    class ResponseEncryptionSpecFactory
    Issuer --> AuthorizeIssuance
    Issuer --> RequestIssuance
    Issuer --> QueryForDeferredCredential
    Issuer --> NotifyIssuer
    Issuer --> CredentialOffer
    Issuer --> DPoPJwtFactory
    Issuer --> DeferredIssuanceContext
    Issuer --> SubmissionOutcome
    SubmissionOutcome --> Deferred
    Issuer --> OpenId4VCIConfig
    Issuer --> HttpClient
    Issuer --> CredentialIssuerId
    Issuer --> CredentialIssuerMetadata
    Issuer --> CIAuthorizationServerMetadata
    Issuer --> KtorHttpClientFactory
    Issuer --> ResponseEncryptionSpecFactory
    '''

    
