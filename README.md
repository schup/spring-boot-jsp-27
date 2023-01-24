# Spring Boot 2.7 sample with JSP

```
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Trying to match request against DefaultSecurityFilterChain [RequestMatcher=any request, Filters=[org.springframework.security.web.session.DisableEncodeUrlFilter@50b92788, org.springframework.security.web.context.request.async.WebAsyncManagerIntegrationFilter@554ed7cf, org.springframework.security.web.context.SecurityContextPersistenceFilter@77a73dbc, org.springframework.security.web.header.HeaderWriterFilter@1ad86a51, org.springframework.security.web.csrf.CsrfFilter@1fc19ebb, org.springframework.security.web.authentication.logout.LogoutFilter@5c57af57, org.springframework.security.web.authentication.UsernamePasswordAuthenticationFilter@f8a45aa, org.springframework.security.web.authentication.ui.DefaultLoginPageGeneratingFilter@419a4097, org.springframework.security.web.authentication.ui.DefaultLogoutPageGeneratingFilter@1b1e39a0, org.springframework.security.web.savedrequest.RequestCacheAwareFilter@4772570c, org.springframework.security.web.servletapi.SecurityContextHolderAwareRequestFilter@236fc184, org.springframework.security.web.authentication.AnonymousAuthenticationFilter@a6821b0, org.springframework.security.web.session.SessionManagementFilter@1b74f00c, org.springframework.security.web.access.ExceptionTranslationFilter@35c52c2, org.springframework.security.web.access.intercept.AuthorizationFilter@538d0745]] (1/1)
DEBUG 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Securing GET /home
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking DisableEncodeUrlFilter (1/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking WebAsyncManagerIntegrationFilter (2/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking SecurityContextPersistenceFilter (3/15)
TRACE 64811 --- [nio-8027-exec-5] w.c.HttpSessionSecurityContextRepository : Did not find SecurityContext in HttpSession 0134557B152E02CC71E249356F78274D using the SPRING_SECURITY_CONTEXT session attribute
TRACE 64811 --- [nio-8027-exec-5] w.c.HttpSessionSecurityContextRepository : Created SecurityContextImpl [Null authentication]
DEBUG 64811 --- [nio-8027-exec-5] s.s.w.c.SecurityContextPersistenceFilter : Set SecurityContextHolder to empty SecurityContext
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking HeaderWriterFilter (4/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking CsrfFilter (5/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.csrf.CsrfFilter         : Did not protect against CSRF since request did not match CsrfNotRequired [TRACE, HEAD, GET, OPTIONS]
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking LogoutFilter (6/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.s.w.a.logout.LogoutFilter            : Did not match request to Ant [pattern='/logout', POST]
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking UsernamePasswordAuthenticationFilter (7/15)
TRACE 64811 --- [nio-8027-exec-5] w.a.UsernamePasswordAuthenticationFilter : Did not match request to Ant [pattern='/login', POST]
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking DefaultLoginPageGeneratingFilter (8/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking DefaultLogoutPageGeneratingFilter (9/15)
TRACE 64811 --- [nio-8027-exec-5] .w.a.u.DefaultLogoutPageGeneratingFilter : Did not render default logout page since request did not match [Ant [pattern='/logout', GET]]
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking RequestCacheAwareFilter (10/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.s.w.s.HttpSessionRequestCache        : No saved request
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking SecurityContextHolderAwareRequestFilter (11/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking AnonymousAuthenticationFilter (12/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.s.w.a.AnonymousAuthenticationFilter  : Set SecurityContextHolder to AnonymousAuthenticationToken [Principal=anonymousUser, Credentials=[PROTECTED], Authenticated=true, Details=WebAuthenticationDetails [RemoteIpAddress=0:0:0:0:0:0:0:1, SessionId=0134557B152E02CC71E249356F78274D], Granted Authorities=[ROLE_ANONYMOUS]]
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking SessionManagementFilter (13/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking ExceptionTranslationFilter (14/15)
TRACE 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Invoking AuthorizationFilter (15/15)
TRACE 64811 --- [nio-8027-exec-5] estMatcherDelegatingAuthorizationManager : Authorizing SecurityContextHolderAwareRequestWrapper[ org.springframework.security.web.header.HeaderWriterFilter$HeaderWriterRequest@7a410026]
TRACE 64811 --- [nio-8027-exec-5] estMatcherDelegatingAuthorizationManager : Checking authorization on SecurityContextHolderAwareRequestWrapper[ org.springframework.security.web.header.HeaderWriterFilter$HeaderWriterRequest@7a410026] using org.springframework.security.config.annotation.web.configurers.AuthorizeHttpRequestsConfigurer$$Lambda$672/0x000000080103e060@7fba2188
DEBUG 64811 --- [nio-8027-exec-5] o.s.security.web.FilterChainProxy        : Secured GET /home
DEBUG 64811 --- [nio-8027-exec-5] org.apache.jasper.servlet.JspServlet     : JspEngine --> /WEB-INF/jsp/home.jsp
DEBUG 64811 --- [nio-8027-exec-5] org.apache.jasper.servlet.JspServlet     : 	     ServletPath: /WEB-INF/jsp/home.jsp
DEBUG 64811 --- [nio-8027-exec-5] org.apache.jasper.servlet.JspServlet     : 	        PathInfo: null
DEBUG 64811 --- [nio-8027-exec-5] org.apache.jasper.servlet.JspServlet     : 	        RealPath: /Users/schup/work/tmp/demo/src/main/webapp/WEB-INF/jsp/home.jsp
DEBUG 64811 --- [nio-8027-exec-5] org.apache.jasper.servlet.JspServlet     : 	      RequestURI: /WEB-INF/jsp/home.jsp
DEBUG 64811 --- [nio-8027-exec-5] org.apache.jasper.servlet.JspServlet     : 	     QueryString: null
TRACE 64811 --- [nio-8027-exec-5] o.s.s.w.header.writers.HstsHeaderWriter  : Not injecting HSTS header since it did not match request to [Is Secure]
DEBUG 64811 --- [nio-8027-exec-5] w.c.HttpSessionSecurityContextRepository : Did not store anonymous SecurityContext
DEBUG 64811 --- [nio-8027-exec-5] w.c.HttpSessionSecurityContextRepository : Did not store anonymous SecurityContext
DEBUG 64811 --- [nio-8027-exec-5] s.s.w.c.SecurityContextPersistenceFilter : Cleared SecurityContextHolder to complete request
```
