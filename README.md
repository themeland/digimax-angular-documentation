# Template customization


## src
I hope you have seen this template `src` folder on the downloaded package `Digimax - Angular 10 SEO & Digital Marketing Agency template` from ThemeForest.

In this `src` folder you can see `index.html` file. This file structure is like this-

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!--meta, title, base, google fonts, all css linking here-->
</head>

<body>

  <app-root></app-root>
 
 <!--all js linking here-->
</body>

</html>
```

All HTML content will be load into this `app-root`:
```html
<app-root></app-root>
```


## entry points

##### app-component.html
Template `app-component.html` structure looks like this-
```html
<router-outlet></router-outlet>

```

##### app-component.ts
Here we have generated all of our components. Template `app-component.ts` structure looks like this-
```js
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'digimax';
}

```

##### app.module.ts
Template `app.module.ts` structure looks like this-
```js
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';

import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';
import { HeaderOneComponent } from './components/header/header-one/header-one.component';
import { HeaderTwoComponent } from './components/header/header-two/header-two.component';
import { HeroOneComponent } from './components/hero/hero-one/hero-one.component';
import { HeroTwoComponent } from './components/hero/hero-two/hero-two.component';
import { HeroThreeComponent } from './components/hero/hero-three/hero-three.component';
import { HeroFourComponent } from './components/hero/hero-four/hero-four.component';
import { HeroFiveComponent } from './components/hero/hero-five/hero-five.component';
import { HeroSixComponent } from './components/hero/hero-six/hero-six.component';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { PromoOneComponent } from './components/promo/promo-one/promo-one.component';
import { PromoTwoComponent } from './components/promo/promo-two/promo-two.component';
import { ContentOneComponent } from './components/content/content-one/content-one.component';
import { ContentTwoComponent } from './components/content/content-two/content-two.component';
import { ContentThreeComponent } from './components/content/content-three/content-three.component';
import { ContentFourComponent } from './components/content/content-four/content-four.component';
import { ContentFiveComponent } from './components/content/content-five/content-five.component';
import { ServiceOneComponent } from './components/services/service-one/service-one.component';
import { ServiceTwoComponent } from './components/services/service-two/service-two.component';
import { ServiceThreeComponent } from './components/services/service-three/service-three.component';
import { ServiceFourComponent } from './components/services/service-four/service-four.component';
import { ServiceFiveComponent } from './components/services/service-five/service-five.component';
import { PortfolioOneComponent } from './components/portfolio/portfolio-one/portfolio-one.component';
import { PortfolioTwoComponent } from './components/portfolio/portfolio-two/portfolio-two.component';
import { PricingOneComponent } from './components/pricing/pricing-one/pricing-one.component';
import { PricingTwoComponent } from './components/pricing/pricing-two/pricing-two.component';
import { PricingThreeComponent } from './components/pricing/pricing-three/pricing-three.component';
import { ReviewOneComponent } from './components/reviews/review-one/review-one.component';
import { ReviewTwoComponent } from './components/reviews/review-two/review-two.component';
import { ContactOneComponent } from './components/contact/contact-one/contact-one.component';
import { ContactTwoComponent } from './components/contact/contact-two/contact-two.component';
import { CtaComponent } from './components/cta/cta.component';
import { FooterOneComponent } from './components/footer/footer-one/footer-one.component';
import { FooterTwoComponent } from './components/footer/footer-two/footer-two.component';
import { ModalSearchComponent } from './components/modal/modal-search/modal-search.component';
import { ModalMenuComponent } from './components/modal/modal-menu/modal-menu.component';
import { ScrollupComponent } from './components/scrollup/scrollup.component';
import { VideoComponent } from './components/video/video.component';
import { BrandingComponent } from './components/branding/branding.component';
import { ServiceSixComponent } from './components/services/service-six/service-six.component';
import { ReviewThreeComponent } from './components/reviews/review-three/review-three.component';
import { HeaderThreeComponent } from './components/header/header-three/header-three.component';
import { ThemeSevenComponent } from './themes/theme-seven/theme-seven.component';
import { ThemeEightComponent } from './themes/theme-eight/theme-eight.component';
import { ThemeNineComponent } from './themes/theme-nine/theme-nine.component';
import { ThemeTenComponent } from './themes/theme-ten/theme-ten.component';
import { ThemeElevenComponent } from './themes/theme-eleven/theme-eleven.component';
import { ThemeTwelveComponent } from './themes/theme-twelve/theme-twelve.component';
import { HeaderFourComponent } from './components/header/header-four/header-four.component';
import { BreadcrumbAboutComponent } from './components/breadcrumb/breadcrumb-about/breadcrumb-about.component';
import { BreadcrumbServicesComponent } from './components/breadcrumb/breadcrumb-services/breadcrumb-services.component';
import { BreadcrumbPortfolioGridComponent } from './components/breadcrumb/breadcrumb-portfolio-grid/breadcrumb-portfolio-grid.component';
import { BreadcrumbPortfolioMinimalComponent } from './components/breadcrumb/breadcrumb-portfolio-minimal/breadcrumb-portfolio-minimal.component';
import { BreadcrumbPortfolioNoGapComponent } from './components/breadcrumb/breadcrumb-portfolio-no-gap/breadcrumb-portfolio-no-gap.component';
import { BreadcrumbPortfolioMasonryComponent } from './components/breadcrumb/breadcrumb-portfolio-masonry/breadcrumb-portfolio-masonry.component';
import { BreadcrumbTeamComponent } from './components/breadcrumb/breadcrumb-team/breadcrumb-team.component';
import { BreadcrumbPricingComponent } from './components/breadcrumb/breadcrumb-pricing/breadcrumb-pricing.component';
import { BreadcrumbContactComponent } from './components/breadcrumb/breadcrumb-contact/breadcrumb-contact.component';
import { BreadcrumbBlogTwoColumnComponent } from './components/breadcrumb/breadcrumb-blog-two-column/breadcrumb-blog-two-column.component';
import { BreadcrumbBlogThreeColumnComponent } from './components/breadcrumb/breadcrumb-blog-three-column/breadcrumb-blog-three-column.component';
import { BreadcrumbBlogLeftSidebarComponent } from './components/breadcrumb/breadcrumb-blog-left-sidebar/breadcrumb-blog-left-sidebar.component';
import { BreadcrumbBlogRightSidebarComponent } from './components/breadcrumb/breadcrumb-blog-right-sidebar/breadcrumb-blog-right-sidebar.component';
import { BreadcrumbBlogDetailsLeftSidebarComponent } from './components/breadcrumb/breadcrumb-blog-details-left-sidebar/breadcrumb-blog-details-left-sidebar.component';
import { BreadcrumbBlogDetailsRightSidebarComponent } from './components/breadcrumb/breadcrumb-blog-details-right-sidebar/breadcrumb-blog-details-right-sidebar.component';
import { AboutComponent } from './components/inner-pages/about/about.component';
import { ServicesComponent } from './components/inner-pages/services/services.component';
import { PortfolioGridComponent } from './components/inner-pages/portfolio/portfolio-grid/portfolio-grid.component';
import { PortfolioMinimalComponent } from './components/inner-pages/portfolio/portfolio-minimal/portfolio-minimal.component';
import { PortfolioNoGapComponent } from './components/inner-pages/portfolio/portfolio-no-gap/portfolio-no-gap.component';
import { PortfolioMasonryComponent } from './components/inner-pages/portfolio/portfolio-masonry/portfolio-masonry.component';
import { TeamComponent } from './components/inner-pages/team/team.component';
import { PricingComponent } from './components/inner-pages/pricing/pricing.component';
import { ContactComponent } from './components/inner-pages/contact/contact.component';
import { ErrorComponent } from './components/inner-pages/error/error.component';
import { BlogTwoColumnComponent } from './components/blogs/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/blogs/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/blogs/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/blogs/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/blogs/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/blogs/blog-details-right-sidebar/blog-details-right-sidebar.component';
import { GoalComponent } from './components/goal/goal.component';
import { TeamOneComponent } from './components/team/team-one/team-one.component';
import { TeamTwoComponent } from './components/team/team-two/team-two.component';
import { ServiceSevenComponent } from './components/services/service-seven/service-seven.component';
import { PortfolioThreeComponent } from './components/portfolio/portfolio-three/portfolio-three.component';
import { PortfolioFourComponent } from './components/portfolio/portfolio-four/portfolio-four.component';
import { PortfolioFiveComponent } from './components/portfolio/portfolio-five/portfolio-five.component';
import { PortfolioSixComponent } from './components/portfolio/portfolio-six/portfolio-six.component';
import { ContactThreeComponent } from './components/contact/contact-three/contact-three.component';
import { PricingFourComponent } from './components/pricing/pricing-four/pricing-four.component';
import { GoogleMapComponent } from './components/google-map/google-map.component';
import { AboutUsComponent } from './components/about-us/about-us.component';
import { BlogOneComponent } from './components/blogs/blog-one/blog-one.component';
import { BlogTwoComponent } from './components/blogs/blog-two/blog-two.component';
import { BlogThreeComponent } from './components/blogs/blog-three/blog-three.component';
import { BlogFourComponent } from './components/blogs/blog-four/blog-four.component';
import { FooterThreeComponent } from './components/footer/footer-three/footer-three.component';
import { BlogFiveComponent } from './components/blogs/blog-five/blog-five.component';
import { BlogSixComponent } from './components/blogs/blog-six/blog-six.component';

@NgModule({
  declarations: [
    AppComponent,
    HeaderOneComponent,
    HeaderTwoComponent,
    HeroOneComponent,
    HeroTwoComponent,
    HeroThreeComponent,
    HeroFourComponent,
    HeroFiveComponent,
    HeroSixComponent,
    ThemeOneComponent,
    ThemeTwoComponent,
    ThemeThreeComponent,
    ThemeFourComponent,
    ThemeFiveComponent,
    ThemeSixComponent,
    PromoOneComponent,
    PromoTwoComponent,
    ContentOneComponent,
    ContentTwoComponent,
    ContentThreeComponent,
    ContentFourComponent,
    ContentFiveComponent,
    ServiceOneComponent,
    ServiceTwoComponent,
    ServiceThreeComponent,
    ServiceFourComponent,
    ServiceFiveComponent,
    PortfolioOneComponent,
    PortfolioTwoComponent,
    PricingOneComponent,
    PricingTwoComponent,
    PricingThreeComponent,
    ReviewOneComponent,
    ReviewTwoComponent,
    ContactOneComponent,
    ContactTwoComponent,
    CtaComponent,
    FooterOneComponent,
    FooterTwoComponent,
    ModalSearchComponent,
    ModalMenuComponent,
    ScrollupComponent,
    VideoComponent,
    BrandingComponent,
    ServiceSixComponent,
    ReviewThreeComponent,
    HeaderThreeComponent,
    ThemeSevenComponent,
    ThemeEightComponent,
    ThemeNineComponent,
    ThemeTenComponent,
    ThemeElevenComponent,
    ThemeTwelveComponent,
    HeaderFourComponent,
    BreadcrumbAboutComponent,
    BreadcrumbServicesComponent,
    BreadcrumbPortfolioGridComponent,
    BreadcrumbPortfolioMinimalComponent,
    BreadcrumbPortfolioNoGapComponent,
    BreadcrumbPortfolioMasonryComponent,
    BreadcrumbTeamComponent,
    BreadcrumbPricingComponent,
    BreadcrumbContactComponent,
    BreadcrumbBlogTwoColumnComponent,
    BreadcrumbBlogThreeColumnComponent,
    BreadcrumbBlogLeftSidebarComponent,
    BreadcrumbBlogRightSidebarComponent,
    BreadcrumbBlogDetailsLeftSidebarComponent,
    BreadcrumbBlogDetailsRightSidebarComponent,
    AboutComponent,
    ServicesComponent,
    PortfolioGridComponent,
    PortfolioMinimalComponent,
    PortfolioNoGapComponent,
    PortfolioMasonryComponent,
    TeamComponent,
    PricingComponent,
    ContactComponent,
    ErrorComponent,
    BlogTwoColumnComponent,
    BlogThreeColumnComponent,
    BlogLeftSidebarComponent,
    BlogRightSidebarComponent,
    BlogDetailsLeftSidebarComponent,
    BlogDetailsRightSidebarComponent,
    GoalComponent,
    TeamOneComponent,
    TeamTwoComponent,
    ServiceSevenComponent,
    PortfolioThreeComponent,
    PortfolioFourComponent,
    PortfolioFiveComponent,
    PortfolioSixComponent,
    ContactThreeComponent,
    PricingFourComponent,
    GoogleMapComponent,
    AboutUsComponent,
    BlogOneComponent,
    BlogTwoComponent,
    BlogThreeComponent,
    BlogFourComponent,
    FooterThreeComponent,
    BlogFiveComponent,
    BlogSixComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```


## themes

`themes` folder included on `app` folder. You can check our folder structure on `app` folder menu.
This is `themes` folder structure-
```text
|-- themes
    |-- theme-one ( default theme)
    |-- theme-two ( demo theme 2)
    .....
    |-- theme-twelve ( demo theme 12 )
```

`themes` folder contains all of our 12 multi-page & one page demos.


## app-routing
In `app` folder we used `app-routing.module.ts`. Where we linked all the route for our all theme. For routing we used angular-router.

Routes: `src/app/app-routing.module.ts`

```js
import { NgModule } from '@angular/core';
import { Routes, RouterModule } from '@angular/router';
import { ThemeOneComponent } from './themes/theme-one/theme-one.component';
import { ThemeTwoComponent } from './themes/theme-two/theme-two.component';
import { ThemeThreeComponent } from './themes/theme-three/theme-three.component';
import { ThemeFourComponent } from './themes/theme-four/theme-four.component';
import { ThemeFiveComponent } from './themes/theme-five/theme-five.component';
import { ThemeSixComponent } from './themes/theme-six/theme-six.component';
import { ThemeSevenComponent } from './themes/theme-seven/theme-seven.component';
import { ThemeEightComponent } from './themes/theme-eight/theme-eight.component';
import { ThemeNineComponent } from './themes/theme-nine/theme-nine.component';
import { ThemeTenComponent } from './themes/theme-ten/theme-ten.component';
import { ThemeElevenComponent } from './themes/theme-eleven/theme-eleven.component';
import { ThemeTwelveComponent } from './themes/theme-twelve/theme-twelve.component';
import { AboutComponent } from './components/inner-pages/about/about.component';
import { ServicesComponent } from './components/inner-pages/services/services.component';
import { PortfolioGridComponent } from './components/inner-pages/portfolio/portfolio-grid/portfolio-grid.component';
import { PortfolioMinimalComponent } from './components/inner-pages/portfolio/portfolio-minimal/portfolio-minimal.component';
import { PortfolioNoGapComponent } from './components/inner-pages/portfolio/portfolio-no-gap/portfolio-no-gap.component';
import { PortfolioMasonryComponent } from './components/inner-pages/portfolio/portfolio-masonry/portfolio-masonry.component';
import { TeamComponent } from './components/inner-pages/team/team.component';
import { PricingComponent } from './components/inner-pages/pricing/pricing.component';
import { ContactComponent } from './components/inner-pages/contact/contact.component';
import { ErrorComponent } from './components/inner-pages/error/error.component';
import { BlogTwoColumnComponent } from './components/blogs/blog-two-column/blog-two-column.component';
import { BlogThreeColumnComponent } from './components/blogs/blog-three-column/blog-three-column.component';
import { BlogLeftSidebarComponent } from './components/blogs/blog-left-sidebar/blog-left-sidebar.component';
import { BlogRightSidebarComponent } from './components/blogs/blog-right-sidebar/blog-right-sidebar.component';
import { BlogDetailsLeftSidebarComponent } from './components/blogs/blog-details-left-sidebar/blog-details-left-sidebar.component';
import { BlogDetailsRightSidebarComponent } from './components/blogs/blog-details-right-sidebar/blog-details-right-sidebar.component';

const routes: Routes = [
  {path: '', component: ThemeOneComponent},
  {path: 'theme-two', component: ThemeTwoComponent},
  {path: 'theme-three', component: ThemeThreeComponent},
  {path: 'theme-four', component: ThemeFourComponent},
  {path: 'theme-five', component: ThemeFiveComponent},
  {path: 'theme-six', component: ThemeSixComponent},
  {path: 'theme-seven', component: ThemeSevenComponent},
  {path: 'theme-eight', component: ThemeEightComponent},
  {path: 'theme-nine', component: ThemeNineComponent},
  {path: 'theme-ten', component: ThemeTenComponent},
  {path: 'theme-eleven', component: ThemeElevenComponent},
  {path: 'theme-twelve', component: ThemeTwelveComponent},
  {path: 'about', component: AboutComponent},
  {path: 'services', component: ServicesComponent},
  {path: 'portfolio-grid', component: PortfolioGridComponent},
  {path: 'portfolio-minimal', component: PortfolioMinimalComponent},
  {path: 'portfolio-no-gap', component: PortfolioNoGapComponent},
  {path: 'portfolio-masonry', component: PortfolioMasonryComponent},
  {path: 'team', component: TeamComponent},
  {path: 'pricing', component: PricingComponent},
  {path: 'contact', component: ContactComponent},
  {path: 'error', component: ErrorComponent},
  {path: 'blog-two-column', component: BlogTwoColumnComponent},
  {path: 'blog-three-column', component: BlogThreeColumnComponent},
  {path: 'blog-left-sidebar', component: BlogLeftSidebarComponent},
  {path: 'blog-right-sidebar', component: BlogRightSidebarComponent},
  {path: 'blog-details-left-sidebar', component: BlogDetailsLeftSidebarComponent},
  {path: 'blog-details-right-sidebar', component: BlogDetailsRightSidebarComponent}
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }

```


## components
Under `components` folder we generated all of our components individually. 
We have generated these components to make the developer’s life easy. 
By using these basic components, For example in our components directory there is `header`, `hero` , `footer` folder where we wrote our different styled component. For example `hero` component-

### Component folder structure
```text
|-- components
    ....
    ..
    |-- hero ( hero component folder )
        - hero-one ( main demo hero section )
        - hero-two ( demo two hero section )
        ...... ( and other )
    ...    
```

### Contact Page component
`inner-pages/contact/contact.component.html`

```text
|-- components
    ....
    ..
    |-- inner-pages ( all inner-pages folder )
        ......
        - contact ( contact-page component )
        ...... ( and other )
    ...    
```

```html
<div class="main overflow-hidden">
    <app-scrollup></app-scrollup>
    <app-header-one></app-header-one>
    <app-breadcrumb-contact></app-breadcrumb-contact>
    <app-contact-one></app-contact-one>
    <app-google-map></app-google-map>
    <app-footer-one></app-footer-one>
    <app-modal-search></app-modal-search>
    <app-modal-menu></app-modal-menu>
</div>
```


## theme installtion
To install the theme you have to install [angular](https://cli.angular.io/) than go to the theme root dir where `package.json` located and use
```bash
npm install -g @angular/cli
```
it will install the packages.

After install process now you can run local server- local server port is 'http://localhost:4200' For developement start use
```bash
ng serve -o
```
## Build your theme
```bash
ng build --prod
```

## For deployment -- static server
First install
```bash
ng build --watch
ng build --aot
```
If you want to know more about static deployment please visit [Angular app deployment](https://angular.io/guide/deployment)

Enjoy your theme :)
