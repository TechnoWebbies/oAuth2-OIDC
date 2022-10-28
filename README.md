# oAuth2-OIDC
Sample Project of oAuth2 and OIDC with Angullar
# Sample-Auth-Server
You can use the OIDC-Sample-Server used in our examples. It assumes, that your Web-App runs on http://localhost:4200

          Username/Password:
                    max/geheim
                    bob/bob
                    alice/alice
                    
          clientIds:
                    spa (Code Flow + PKCE)
                    implicit (implicit flow)
          redirectUris:
                    localhost:[4200-4202]
                    localhost:[4200-4202]/index.html
                    localhost:[4200-4202]/silent-refresh.html

# Installing
          npm i angular-oauth2-oidc --save

# Importing the NgModule
          import { HttpClientModule } from '@angular/common/http';
          import { OAuthModule } from 'angular-oauth2-oidc';

          @NgModule({
            imports: [
              // etc.
              HttpClientModule,
              OAuthModule.forRoot()
            ],
            declarations: [
              AppComponent,
              HomeComponent,
              // etc.
            ],
            bootstrap: [
              AppComponent
            ]
          })
          export class AppModule {
          }
