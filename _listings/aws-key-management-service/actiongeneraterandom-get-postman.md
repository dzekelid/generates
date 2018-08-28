{
  "info": {
    "name": "AWS Key Management Service API Generate Random",
    "_postman_id": "d17c6331-c652-4f2f-a948-fd2bd0181ed2",
    "description": "Generates an unpredictable byte string.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Keys",
      "item": [
        {
          "id": "02d88aaf-1849-4235-8009-ee468c25d87f",
          "name": "cancelKeyDeletion",
          "request": {
            "url": "http://example.com/api/?Action=CancelKeyDeletion?KeyId=KeyId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels the deletion of a customer master key (CMK)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59f92069-3a1f-4e64-804e-17a1cf1e66a9"
            }
          ]
        },
        {
          "id": "b0cfebe7-38c7-4acb-8ab0-805243d95d1a",
          "name": "createKey",
          "request": {
            "url": "http://example.com/api/?Action=CreateKey?BypassPolicyLockoutSafetyCheck=BypassPolicyLockoutSafetyCheck&Description=Description&KeyUsage=KeyUsage&Origin=Origin&Policy=Policy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a customer master key (CMK)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8a7fc99-6306-466c-a6d4-94f10a081f9c"
            }
          ]
        },
        {
          "id": "7abf82c9-4aa6-4040-bfbe-02292416b4e1",
          "name": "deleteImportedKeyMaterial",
          "request": {
            "url": "http://example.com/api/?Action=DeleteImportedKeyMaterial?KeyId=KeyId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes key material that you previously imported and makes the specified customer\n      master key (CMK) unusable."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbcee56b-2c5e-4fed-bda0-91d4f683431b"
            }
          ]
        },
        {
          "id": "737be787-105f-4a8e-9bda-06fde636392e",
          "name": "describeKey",
          "request": {
            "url": "http://example.com/api/?Action=DescribeKey?GrantTokens=GrantTokens&KeyId=KeyId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides detailed information about the specified customer master key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "942a7d0a-469c-45e4-8253-43f6c116c29b"
            }
          ]
        },
        {
          "id": "1ff4f524-cd86-4572-8009-55f4368af508",
          "name": "disableKey",
          "request": {
            "url": "http://example.com/api/?Action=DisableKey?KeyId=KeyId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the state of a customer master key (CMK) to disabled, thereby preventing its use\n      for cryptographic operations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "080b01da-82fd-4ab3-b336-75cd6643f4d7"
            }
          ]
        },
        {
          "id": "1ba29fbd-548f-4667-a00b-1bc624058fa9",
          "name": "disableKeyRotation",
          "request": {
            "url": "http://example.com/api/?Action=DisableKeyRotation?KeyId=KeyId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables rotation of the specified key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "083ed339-07aa-420a-8970-23c8f161657f"
            }
          ]
        },
        {
          "id": "7369d072-8076-4978-83ca-fe4844f50e95",
          "name": "enableKey",
          "request": {
            "url": "http://example.com/api/?Action=EnableKey?KeyId=KeyId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Marks a key as enabled, thereby permitting its use."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdd9eb85-2b70-4282-a7af-0a474b363171"
            }
          ]
        },
        {
          "id": "a5f78f2d-2af2-4f3f-8438-8951a6adbf2c",
          "name": "enableKeyRotation",
          "request": {
            "url": "http://example.com/api/?Action=EnableKeyRotation?KeyId=KeyId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables rotation of the specified customer master key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6908294f-f5cf-4089-804f-0003bc891405"
            }
          ]
        },
        {
          "id": "643fa19c-a727-4a13-b512-8e4670f7974e",
          "name": "generateDataKey",
          "request": {
            "url": "http://example.com/api/?Action=GenerateDataKey?EncryptionContext=EncryptionContext&GrantTokens=GrantTokens&KeyId=KeyId&KeySpec=KeySpec&NumberOfBytes=NumberOfBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a data encryption key that you can use in your application to encrypt\n      data locally."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab1a2e40-42f4-448e-8348-c3b6c9efcf76"
            }
          ]
        },
        {
          "id": "1869d28e-8401-4cf2-9a09-cd67d23218fc",
          "name": "generateDataKeyWithoutPlaintext",
          "request": {
            "url": "http://example.com/api/?Action=GenerateDataKeyWithoutPlaintext?EncryptionContext=EncryptionContext&GrantTokens=GrantTokens&KeyId=KeyId&KeySpec=KeySpec&NumberOfBytes=NumberOfBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a data encryption key encrypted under a customer master key (CMK)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b273c927-c06f-4688-baaa-71f2da111cb8"
            }
          ]
        }
      ]
    },
    {
      "name": "Aliases",
      "item": [
        {
          "id": "71ab280a-d31e-483e-9c7d-8893d45321d1",
          "name": "createAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAlias?AliasName=AliasName&TargetKeyId=TargetKeyId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a display name for a customer master key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22da00bc-7bba-43a2-97e5-1a7ad60f3af8"
            }
          ]
        },
        {
          "id": "2165341a-bded-4026-8fd0-be74dd2b4b58",
          "name": "deleteAlias",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAlias?AliasName=AliasName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified alias."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d80f5d4d-1eb9-4812-b6b8-6f751c27c9a5"
            }
          ]
        }
      ]
    },
    {
      "name": "Grants",
      "item": [
        {
          "id": "67844ab6-e70e-411b-8b4f-1b5e372d1bab",
          "name": "createGrant",
          "request": {
            "url": "http://example.com/api/?Action=CreateGrant?Constraints=Constraints&GranteePrincipal=GranteePrincipal&GrantTokens=GrantTokens&KeyId=KeyId&Name=Name&Operations=Operations&RetiringPrincipal=RetiringPrincipal",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a grant to a key to specify who can use the key and under what conditions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb28318a-c2eb-4e3a-863d-6bf96e7731da"
            }
          ]
        }
      ]
    },
    {
      "name": "Decrypt",
      "item": [
        {
          "id": "4f110afd-c009-494f-aded-b7e27c64738e",
          "name": "decrypt",
          "request": {
            "url": "http://example.com/api/?Action=Decrypt?CiphertextBlob=CiphertextBlob&EncryptionContext=EncryptionContext&GrantTokens=GrantTokens",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Decrypts ciphertext."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b18de652-41d4-4c4e-98d3-1a3660725ac1"
            }
          ]
        }
      ]
    },
    {
      "name": "Encrypt",
      "item": [
        {
          "id": "05f74711-b65d-413a-8bd3-e4da11cf8926",
          "name": "encrypt",
          "request": {
            "url": "http://example.com/api/?Action=Encrypt?EncryptionContext=EncryptionContext&GrantTokens=GrantTokens&KeyId=KeyId&Plaintext=Plaintext",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Encrypts plaintext into ciphertext by using a customer master key."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03ae6568-f580-4f48-ab0a-f28097041623"
            }
          ]
        }
      ]
    },
    {
      "name": "Randoms",
      "item": [
        {
          "id": "87e4768b-68de-4682-9bfa-4cfcea0fc437",
          "name": "generateRandom",
          "request": {
            "url": "http://example.com/api/?Action=GenerateRandom?NumberOfBytes=NumberOfBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates an unpredictable byte string."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eff2a3be-22f7-460e-80f7-dd5f913412ba"
            }
          ]
        }
      ]
    }
  ]
}