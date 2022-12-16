# FT Setup for Mobius

1. first make sure you have cloned both [mobius repo](https://sqbu-github.cisco.com/webrtc-calling/mobius) and [mobius functional test repo](https://sqbu-github.cisco.com/webrtc-calling/mobius-functional-tests) 
2. create tests branch in both repos 
    
    ```powershell
    git checkout -b "testbranch name" main
    ```
    
3. go to `SipAppConfigProperties.java` in your mobius repo </br></br>
   a. Replace `getSipCertificate()`  to
    
    ```java
    @Override
        public String getSipCertificate() {
            return "-----BEGIN CERTIFICATE-----\n" +
                    "MIIE5TCCA82gAwIBAgIJAK3u4WUSgTLcMA0GCSqGSIb3DQEBCwUAMDAxCzAJBgNV\n" +
                    "BAYTAlVTMSEwHwYDVQQDDBhNb2JpdXPDosKAwpRUZXN0LVJvb3QtQ0EwHhcNMjIx\n" +
                    "MDE5MTExNjIwWhcNMjMxMDE5MTExNjIwWjBBMQswCQYDVQQGEwJJTjELMAkGA1UE\n" +
                    "CAwCS0ExDjAMBgNVBAoMBUNpc2NvMRUwEwYDVQQLDAxXZWJleENhbGxpbmcwggIi\n" +
                    "MA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQCZxP02qNnlmq8921CDzDDa3fN4\n" +
                    "kPnNoOwRmq15D6Azcn/i9r8eEr48d1wIsUmeubXZKtmXyEBUSAfo1YGvMNupQHCZ\n" +
                    "tlH9GbYHU1cpz+rm1PtSb4FW+wF8ROrgnQ63MoRVejY79ibLNeSt2XxejwuuThuI\n" +
                    "9/Hicc9mJKgrFSv8LPF2CuiHgvL5nXvYJaQ5ZYHfVQlrIEOrtYp9VFx6SQhFlEqn\n" +
                    "Zis8hM0M4wCIIDjG4aIrUjI+35cgMM19AVGic3hh+dPLFfzLjrg9K3KiOnHWe6DX\n" +
                    "M+Fvy7G1j21NWuGE18IXBgXPg5fKGdnvQbQeFh4O765/YqGHLHKVeID9DEYPF2bp\n" +
                    "dIGX4r6XSFk5aJ1OJ/lBuJsD2is5JfGdlkJX6uktozU/wayF+UZ7x+nn9XIBdMVk\n" +
                    "p/JMUCH05zr+kkXpIoH30AAAvqOTJv6noklQlaIk1I+wQV4CfHDPe/HRVxgz9ez3\n" +
                    "HWMBtkLb7hOl8pfrkWdfFKqnPud1mzoNtcZjxnLZKdYffiV3iYhPDprBqE1Z1fO9\n" +
                    "nnAgZhX10V/eyijHZlpKX3HxEXtFrtNbQysV9jKQRYLBWm8ii7hcEffqGrLqBCDZ\n" +
                    "K2D3PKgo7JEU8wViaiDM5GMPOKc3P43BBV+dSDICPDgMA5BESofYSzYyjU2YG20z\n" +
                    "3xHE8tZEG0d/S3TXtQIDAQABo4HwMIHtMAkGA1UdEwQCMAAwEQYJYIZIAYb4QgEB\n" +
                    "BAQDAgWgMDMGCWCGSAGG+EIBDQQmFiRPcGVuU1NMIEdlbmVyYXRlZCBDbGllbnQg\n" +
                    "Q2VydGlmaWNhdGUwHQYDVR0OBBYEFJAd5yx6WFhSObI5Ucv9wtda/55/MEoGA1Ud\n" +
                    "IwRDMEGhNKQyMDAxCzAJBgNVBAYTAlVTMSEwHwYDVQQDDBhNb2JpdXPDosKAwpRU\n" +
                    "ZXN0LVJvb3QtQ0GCCQD1Oyv17L7S2DAOBgNVHQ8BAf8EBAMCBeAwHQYDVR0lBBYw\n" +
                    "FAYIKwYBBQUHAwIGCCsGAQUFBwMEMA0GCSqGSIb3DQEBCwUAA4IBAQBkJB1G+EAw\n" +
                    "tKZW3sHhfppjHDoUN6xj2RCkQKFgScDdzN6JH0GXLpxkQ69V6kiSA7bsT2nlN/52\n" +
                    "xStjqza3Apyn34mPL4jwi2kVSGsZVia/+usYXkOl7f8dfDJbTaq4FeGlqnWEgxiN\n" +
                    "OpBr0ff9Gz7tUagOYwtY/G6sINtw4wVx6RVv+79rrwkn6u7HBHL37YyTyefR646S\n" +
                    "pnfHpz9TA9vQ4XgTphAF3to+Y1DZSnvhcKHTZzEp9z+PsP1SmU5146mBZJW41wM8\n" +
                    "a40CiHoWm1mVw4cS+jA9dkUF+rUFCaR4xJeRPFR8vSggm2UwxWV7mAU66wg1lhP8\n" +
                    "PLlVv0zx/Um1\n" +
                    "-----END CERTIFICATE-----";
            //return env.getProperty("sipCertificate");
        }
    ```
    
   b. Repalce `getSipPrivateKey`()  to 
    
    ```java
    @Override
        public String getSipPrivateKey() {
            //return env.getProperty("sipPrivateKey");
            return "-----BEGIN RSA PRIVATE KEY-----\n" +
                    "MIIJKAIBAAKCAgEAmcT9NqjZ5ZqvPdtQg8ww2t3zeJD5zaDsEZqteQ+gM3J/4va/\n" +
                    "HhK+PHdcCLFJnrm12SrZl8hAVEgH6NWBrzDbqUBwmbZR/Rm2B1NXKc/q5tT7Um+B\n" +
                    "VvsBfETq4J0OtzKEVXo2O/YmyzXkrdl8Xo8Lrk4biPfx4nHPZiSoKxUr/Czxdgro\n" +
                    "h4Ly+Z172CWkOWWB31UJayBDq7WKfVRcekkIRZRKp2YrPITNDOMAiCA4xuGiK1Iy\n" +
                    "Pt+XIDDNfQFRonN4YfnTyxX8y464PStyojpx1nug1zPhb8uxtY9tTVrhhNfCFwYF\n" +
                    "z4OXyhnZ70G0HhYeDu+uf2KhhyxylXiA/QxGDxdm6XSBl+K+l0hZOWidTif5Qbib\n" +
                    "A9orOSXxnZZCV+rpLaM1P8GshflGe8fp5/VyAXTFZKfyTFAh9Oc6/pJF6SKB99AA\n" +
                    "AL6jkyb+p6JJUJWiJNSPsEFeAnxwz3vx0VcYM/Xs9x1jAbZC2+4TpfKX65FnXxSq\n" +
                    "pz7ndZs6DbXGY8Zy2SnWH34ld4mITw6awahNWdXzvZ5wIGYV9dFf3soox2ZaSl9x\n" +
                    "8RF7Ra7TW0MrFfYykEWCwVpvIou4XBH36hqy6gQg2Stg9zyoKOyRFPMFYmogzORj\n" +
                    "DzinNz+NwQVfnUgyAjw4DAOQREqH2Es2Mo1NmBttM98RxPLWRBtHf0t017UCAwEA\n" +
                    "AQKCAgB1ibUABftg3Wdcgfq+c+NYOVX07+RygLJSFojJQ99x0/DbXT7jTvJpJ9eK\n" +
                    "sXGTyWKuWGmw8pnxkomxORqC/na5ng8z/8AWFoQkf1jeFhb5UQ22ipM0GHOfONLM\n" +
                    "1GC+OfgbmmpAVTx8Enr1RIwjf3YvS3cSsGwNam9dJWICZJGVlgkP8PCjPL5bfTyA\n" +
                    "EO3CDcxDGS4025m+c+sjN8vkkVSoUtzprlgYT26pjg8G/pJHu4sJUDAmDSTor0Uz\n" +
                    "a0GqSldXlO6Giw0Lz9EWuNJMHR6NEzzzoq2MlggFv1eOTIybzYyHqsvgPjdVfYMv\n" +
                    "tmpmoQNi6WTZ7FuKBrijdlQqmSonCao8WUUdhVI4K7azGNCzIDoNcHDRdsNRkSZ3\n" +
                    "T/LpiWYhNdzKwaGRcZt60Pn/X9NaC2NRfCaLKK4xKgmaLRFl/9VLBwLclF6fgnEh\n" +
                    "R3Ymq33M2dmfbuQV2IfdCCnStdHymIngjDyJRTknQ/y8dfYaCgZEoE3f1FR7RNPI\n" +
                    "Ittfps1T6XCkGmt7gEiUz73kS2F65Ji54N/Du9IUAqFdtctH3Ik1wdppSuoAO3Rw\n" +
                    "57wOWP1qmPFVkxtJSd7gbRcjx45CxojNE8ZjdMTdKggiCICO1Hj14fRJUvswE1NR\n" +
                    "18WlTOFYuQbkduehUul0/R69op8WOmih7R1UGPtqxffLQxY4QQKCAQEAx6FDFhWv\n" +
                    "m4YZhjoDQqfBYK9QIZ32ZS1wOymiEe5aT2uZYf2QbIFwvncHsYC4wxxQB6HXPaTH\n" +
                    "pyP6tcoUTrCc0/E+gIrLEHtKjGmIrzfWkwzesVCgn1nKm7RgO7+/eA0UtlbsZ4TS\n" +
                    "C8ME9A5dPsLp9m2SVFrKe+zUM4yO+nOM/50vcgk+HfnLL8KSw6iVh+2VhSiwtrFs\n" +
                    "aBRf6NEEuQ6FcL2kAx2BhX/Nwts6tUXDJCq2MsSph9gvLDFnkprzrZOclIZmJRy/\n" +
                    "6SwGzpK3j9L1xQe3QTJW/ezlD9EtH3klYyfhWOCGK7q7rB1Zsi8N3zvdTY6O8IMu\n" +
                    "MSM2x6q/ezjK8QKCAQEAxTCXxXFODCMGh8sxtwvlw6t6/Ncie52KggKEvH6ALHif\n" +
                    "x0vTlTqvK9UeXX2o1SkDtA1yKOAoCkJzbbFNvMvdi5dGpjSiDuOWKuDl0Dv9Ci4A\n" +
                    "49Hx16V1ofE7MS1b2DPYBhZ6c5JaHQIzZUFFerteMWaVl8o3pFn5qHsmDgFnZaMS\n" +
                    "knTjfGRJEwKBsQAAKUcBj+Gzr83tvEnwHJV+U3hPJ7Z8aPON2WLpAplqk3DO+DdJ\n" +
                    "pPQTVWIVK/vjILe41q4jdgjDFE/xa/Dsl6719QLPZBITlWREBm/MIXYphEQDB6X0\n" +
                    "Ft70BvC20XQeIgqRhF7mpd9GtviXLy9Mv5rseQzxBQKCAQA8hbKOFoMH9q70V9A3\n" +
                    "PB7PjjcQChDyecUl2qhtIUM2AtwcrkBD9TZWOEYX1Xuug33r4nAcG0IAdVMEHEDt\n" +
                    "3nOdee1GEU4hMA/Y5AHxhU9Dg8pcHaKkzRc0/4mRc7+7yNN3uICxnb4EnNp6l4RD\n" +
                    "i9pcwLl1Y5Ux3woymrGaUr/zmxcQTqcLdXjZgPb35Lt421nSZhS1PrMsFslBD2WM\n" +
                    "KU/hb00zOJXVAHtEUSzKWl0gMObOG3t+WNdsYYoSE3I/NJprGRgMtlukeJmTtT17\n" +
                    "mCy00HMJjBZ9o32KvxMcEKF6H1Qdmuxyg4l0U+2mrMda345nfgnt9wdhFFj+TdEB\n" +
                    "raUxAoIBAQC6IFfhwkVNJ3JuktlmUhCaVS5NojOmQtoORZpM4YrSbzlBwM0COtZF\n" +
                    "pXB4BrhqG8CnH1n2Qz8IEBksHQOnhTalIDFLiLq/GwsPhiDmIPmDtlCYuf5w8njK\n" +
                    "VwzsKkhbFvR9KpKCrE3qu70PgkC2zEzojE//apyCwXrqEPOmnKSgRwCsxTBEpdRj\n" +
                    "4SXRkJKWY7ORwBT/iH0yEQhXsrP+zbzJW3KrDdmCq94M2grDCOQTXvxgexIUsfQS\n" +
                    "BDwrEb+iw9QtAbBBaAQVQt/PfRIkJnbjmjxp8q5S9QvVOdeORTQm7/op7GCifGvT\n" +
                    "4KrgruET9Q/42XvCEXuCyj7DTNSQniqRAoIBAGn2JvTMFsOWTqn/6kZv7/cVIaaw\n" +
                    "i3zlzDe1olH5DYXxHLiRMRE0udGAJBol6+TC+szfDg+K3nt6aEcIClSQl5brUCG/\n" +
                    "CEBsWDH8nhTRFLc1nCyPb82ebUSjPRzVyBMu70JD/LozjKI0+Dm9NopnxJKZ4KIe\n" +
                    "yVewCQOdkZmU0qgOSUn5skMuLqo0w7mLiFkPfjHUguPS3CCni7ujZjpNfDScxcLb\n" +
                    "4SnueZz+iISejUa80a7/PEfHqmjng603MGqsG2erLXlKN7yxgv0RSWLfTNnEFT9a\n" +
                    "KJTEnc929i+fPdxEyfTtg9uxLpmlF0oN53nGzh6EwrFpw4L3PiOuzFxVnfw=\n" +
                    "-----END RSA PRIVATE KEY-----";
        }
    ```
    
4. then open Tomcat Configuration and in “Starup/Connection” section paste this text


    >OptionsIntervalInSecs=1000000;OptionsDelayInSec=1000000;mobiusClientId=C3d24312bf8cc32b7dc6a839b9de2d6234170ad709e27bd4c0b5e6b6f36e211b0;mobiusClientSecret=2c99f6c16a0045dd5b0eee8bef552fe71f4eea1163be41dc6bec251a24ef5812;mobiusOrgId=a93dde14-65b7-4a59-81dd-28962a8473e3;mobiusPassword=94]W0,Y)zefFQ+2gkM!dD=13v$N7xK1_;mobiusRefreshToken=MTJmN2YzMWUtYTdjYi00NzBkLTlmMzgtYmIyMmFjMmRhNWIyZDMyZTA1ZWUtOTE0_A52D_a93dde14-65b7-4a59-81dd-28962a8473e3;mobiusUsername=webrtcMobius.aintgen-a-1;keepaliveIntervalSeconds=30000;inactivityTimerSeconds=60000;RegExpires=600;OUTBOUND_PROXY_DEFAULT_VALUE=localhost:8899;cpapiServicePublicUrl=[http://localhost:3467/cpapi/api/v1;cxapiServicePublicUrl=http://localhost:3467/cxapi/api/v1](http://localhost:3467/cpapi/api/v1;cxapiServicePublicUrl=http://localhost:3467/cxapi/api/v1)

5.  Run `mvn clean package -DskipTests`  in your mobius directory terminal
6. Now go to your mobius-functional-test repo and copy thses 3 certificates in `functional-tests/src/main/resources` 
Link for the Files -[Here](https://cisco-my.sharepoint.com/:f:/g/personal/ravingup_cisco_com1/EkIH87mK_KdJimlBo5lEk4UBG7-ggXYXXP_k-2X4acAj2Q?e=aYsFq2)
7. Now go to your mobius-functional-test repo and copy thses 3 certificates in `functional-stubs/sse/sse-infra/src/main/resources/certs/grpc` 
Link for the Files -[Here](https://cisco-my.sharepoint.com/personal/ravingup_cisco_com1/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fravingup%5Fcisco%5Fcom1%2FDocuments%2FMobius%2FFT%20Setup%2FCertificate%20%2DCPAPI&ga=1)
8. Go to your repo in termianl and do `pwd` and copy the path 
9. Follow these changes </br>
    <aside>
    💡 You can replace `/Users/ravingup/Downloads/mobius-functional-tests/` with your `path`
    </aside>
  
    1. Now go to `functional-stubs/cpapi-stub/src/main/java/com/ciscospark/mobius/cpapi/CpapiClientTestConfig.java` on line no 13

        ```java
        -@PropertySource({"file:cpapi-stub/src/main/resources/application.properties"})
        +@PropertySource({"file:/Users/ravingup/Downloads/mobius-functional-tests/functional-stubs/cpapi-stub/src/main/resources/application.properties"})
        ```
        
    2. Go to  `functional-stubs/cpapi-stub/src/main/java/com/ciscospark/mobius/cpapi/TestNgApp.java` on line no  14

        ```java
        -        Path path = Paths.get("./cpapi-stub/src/main/resources/testng.xml");
        +        Path path = Paths.get("/Users/ravingup/Downloads/mobius-functional-tests/functional-stubs/cpapi-stub/src/main/resources/testng.xml");
        ```
        
    3. Go to `functional-stubs/cpapi-stub/src/main/resources/application.properties` </br>
       </br>Line no  3

        ```java
        -pingUrl = http://webrtc-mobius-j2.cisco.com:8080/api/v1/ping
        +pingUrl = http://localhost:8080/war_war/api/v1/ping
        ```
        where `[http://localhost:8080/war_war](http://localhost:8080/war_war)` is same as you use in your tomcat URL

        </br>Line no 13
        
        ```java
        -jsonFileLocation = /cpapi-stub/src/main/resources
        +jsonFileLocation = functional-stubs/cpapi-stub/src/main/resources
        ```
        
    4. Go to `functional-stubs/sse/common-sip-pkts/src/main/java/com/cisco/edge/v2/sip/endpoint/AbstractSipEndpoint.java` on line no 173

        ```java
        -                remoteConnection.getLocalIpAddress(), remoteConnection.getLocalPort()));
        +                "0.0.0.0", remoteConnection.getLocalPort()));
        ```
        
    5. Go to `functional-stubs/sse/sse-infra/src/main/java/com/cisco/edge/sbctest/v2/sip/endpoint/CoreEndpoint.java` 
    
       </br>Line no  53

        ```java
        -      Path path = Paths.get("functional-stubs/sse/sse-infra/src/main/resources/certs/server.crt").toAbsolutePath();
        +      Path path = Paths.get("/Users/ravingup/Downloads/mobius-functional-tests/functional-stubs/sse/sse-infra/src/main/resources/certs/server.crt").toAbsolutePath();
        ```
        
        Line no 55
        
        ```java
        -      path = Paths.get("functional-stubs/sse/sse-infra/src/main/resources/certs/server.key").toAbsolutePath();
        +      path = Paths.get("//Users/ravingup/Downloads/mobius-functional-tests/functional-stubs/sse/sse-infra/src/main/resources/certs/server.key").toAbsolutePath();
        ```
        
        Line no 59
        
        ```java
        -      path = Paths.get("functional-stubs/sse/sse-infra/src/main/resources/certs/MobiusRootCA.crt").toAbsolutePath();
        +      path = Paths.get("/Users/ravingup/Downloads/mobius-functional-tests/functional-stubs/sse/sse-infra/src/main/resources/certs/MobiusRootCA.crt").toAbsolutePath();
        ```
        
    6.  go to `functional-tests/src/main/java/com/ciscospark/mobius/ft/MobiusClientTestConfig.java` on line no  27

        ```java
        -@PropertySource({"file:functional-tests/src/main/resources/application.properties"})
        +@PropertySource({"file:/Users/ravingup/Downloads/mobius-functional-tests/functional-tests/src/main/resources/application.properties"})
        ```
        
    7. Go to `functional-tests/src/main/resources/application.properties` 
    
       </br>Line no  18

        ```java
        -mobiusUrl=http://webrtc-mobius-j2.cisco.com:8080/api/v1/calling/web
        +mobiusUrl=http://localhost:8080/war_war/api/v1/calling/web
        ```
        line no 30
        
        ```java
        -FT_USER_1_EMAIL=atlas.test.wxcwebrtc+ft1@gmail.com
        +FT_USER_1_EMAIL= <your testing id>
        +FT_USER_1_USERID= <your UUID>
        +FT_USER_1_PASSWORD= <password>
        +WDM_DEVICE_ID= <device id>
        ```

        ####  `For getting UserId and Device ID`
    
        - Go to [Webex-int](https://web-int.webex.com/calling)  and open inspect in your browser
        - Refer this

            <img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F7347e419-487c-493c-92b2-aec79d9641b0%2FNEW.png?id=61eaeae3-cebe-4c56-a50b-2d210d74a003&table=block&spaceId=7efc9fc5-ab1f-4a88-8b52-44c2ff1a60cc&width=2000&userId=7cc1c975-1d6b-4122-97a1-267d3c91e71d&cache=v2" width="600" height="350"/>
            
    
10.  go to `functional-stubs/cpapi-stub/src/main/java/com/ciscospark/mobius/cpapi/MainApplication.java` and run Main Application 
11. run mobius with redis 
12. Now You can run any testcase