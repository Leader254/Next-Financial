
**Dynamic and Static Rendering**
***Static rendering*** - 
The content of the web pages is generated at build time.
The HTML,CSS, and Javascript are pre-rendered before deployment.
Static rendering is useful for UI with no data that is shared across users, such as a static blog post or a product page.
**Benefits**

 1. Faster Websites - Prerendered content can be cached and globally   
        distributed. 
 2. Reduced Server Load - Because the content is cached,   
        your server does not have to dynamically generate content for each  
        user request. 
  3. SEO - Prerendered content is easier for search engine 
        crawlers to index, as the content is already available when the page
        loads. This can lead to improved search engine rankings.
        
***Dynamic rendering*** - The content of the web pages is rendered on the server for each user request time(When the user visits the page).
**Benefits**

1. Real-Time Data - Dynamic rendering allows your application to display real-time or frequently updated data.
2. User-Specific Content - It's easier to serve personalized content - such as dashboards or user profiles.
3. Request-Time Information - Dynamic rendering allows you to access information that can only be known at request time

**Streaming**
Streaming is a data transfer technique that allows you to break down a route into smaller "chunks" and progressively stream them for the server to the client as they become ready.
***loading.tsx file***
It is a special Next.js file built on top of Suspense, it allows you to create fallback UI to show as a replacement while page content loads.

***useSearchParams hook***
Allows you to access the parameters of the current URL. For example, the search params for this URL `/dashboard/invoices?page=1&query=pending` would look like this: `{page: '1', query: 'pending'}`
***usePathname hook***
It lets you read the current URL's pathname. For example, for the route `/dashboard/invoices`, usePathname would return `'/dashboard/invoices'`.
***useRouter hook***
Enables navigation between routes within client components programmatically.