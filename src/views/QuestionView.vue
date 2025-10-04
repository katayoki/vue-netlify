<style>
.custom-body {
  display: block !important;
  place-items: initial !important;
  max-width: none !important;
  margin: 0 !important;
}
.custom-body #app {
  max-width: none !important;
  margin: 0 !important;
  padding: 0 !important;
  width: 100% !important;
  display: block !important;
}
@media (min-width: 1024px) {
  .custom-body #app {
    display: block !important;
    grid-template-columns: none !important;
    padding: 0 !important;
  }
}
</style>

<template>
  <div class="min-h-screen bg-gray-50 p-6 sm:p-10">
    <header class="mb-8 text-center">
      <h1 class="text-4xl font-extrabold text-gray-900 mb-2">Question and Answer Assessment</h1>
    </header>

    <div class="mx-auto grid gap-8 md:grid-cols-2 lg:grid-cols-3 px-4 sm:px-6 lg:px-50">
      <div
        class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 lg:col-span-3"
      >
        <h3 class="text-xl font-semibold text-indigo-600 mb-3">
          1. Talk about how you made your site and why you chose the tools you did. Briefly explain
          one challenge you experienced in setting up this site and how you overcame it
        </h3>
        <p class="text-gray-700 leading-relaxed text-sm">
          This was my first time using Netlify. I initially attempted a Laravel app but switched to
          Vue.js after realizing PHP wasn’t natively supported on the platform. The shift to Vue
          made deployment seamless and quick—about 10 minutes from local setup to Netlify deployment
          via GitHub.
          <br /><br />
          My main challenge was assuming Laravel (PHP) would run on Netlify. I overcame this by
          consulting the documentation, identifying the limitation, and adjusting my stack to the
          fully supported Vue.js framework.
        </p>
      </div>

      <div
        class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 lg:col-span-3"
      >
        <h3 class="text-xl font-semibold text-indigo-600 mb-3">
          2. What did you think of our service during the time you used it? Provide some
          constructive criticism or some features that impressed you.
        </h3>
        <p class="text-gray-700 leading-relaxed text-sm">
          I found the whole process with Netlify to be smooth and very easy to follow, especially
          after consulting the documentation. What truly impressed me was the Platform’s UI. It is
          clean, well-organized, and highly intuitive, which makes deployment feel seamless even for
          a first-time user. The simplicity of the interface is a major strength.
        </p>
      </div>

      <div
        class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 lg:col-span-3"
      >
        <h3 class="text-xl font-semibold text-indigo-600 mb-3">
          3. Rank your 5 favorite and 5 least favorite activities from this list:
          <a
            href="https://gist.github.com/laurajodz/592402a6336410377dee1a744af846ab"
            class="block text-blue-500 mt-1 break-all"
            target="_blank"
          >
            https://gist.github.com/laurajodz/592402a6336410377dee1a744af846ab
          </a>
        </h3>
        <div class="flex space-x-4">
          <div class="w-1/2">
            <h4 class="font-bold text-green-700 mb-2 border-b pb-1">5 Favorite ⭐</h4>
            <ul class="list-disc list-inside text-gray-700 text-sm space-y-1">
              <li>
                Debug a customer's build using a programming language and framework that you've
                never seen before
              </li>
              <li>Develop a code example to share with a customer</li>
              <li>
                Work with the development team to help design a new feature based on feedback from
                customers
              </li>
              <li>Set up your own copy of several site frameworks for debugging</li>
              <li>Suggest and champion improvements to Support workflow</li>
            </ul>
          </div>
          <div class="w-1/2">
            <h4 class="font-bold text-red-700 mb-2 border-b pb-1">5 Least Favorite ❌</h4>
            <ul class="list-disc list-inside text-gray-700 text-sm space-y-1">
              <li>Respond to 20+ support requests via email every day</li>
              <li>Respond to Netlify customers on Twitter</li>
              <li>
                Engage multiple users at once via chat to answer their questions and troubleshoot
                problems
              </li>
              <li>Help manage communications during a service outage</li>
              <li>Manage a Support team</li>
            </ul>
          </div>
        </div>
      </div>

      <div
        class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 lg:col-span-3"
      >
        <h3 class="text-xl font-semibold text-indigo-600 mb-3">
          4. Provide a link to documentation for a technical/developer-focused product, which you
          think are well done, and explain why you think they are well done
        </h3>
        <p class="text-gray-700 leading-relaxed text-sm">
          I would point to
          <a
            href="https://laravel.com/docs/12.x/installation"
            class="text-blue-500 mt-1"
            target="_blank"
          >
            Laravel’s documentation</a
          >
          as an excellent example of well-done developer-focused docs. What makes it stand out is
          its clarity, organization, and the way it caters to both beginners and experienced
          developers. Each feature is explained step by step with practical code examples, making it
          easy to follow and apply immediately in real projects.
          <br /><br />
          In addition, the Laravel ecosystem reinforces the documentation with resources like
          Laracasts, tutorials, and related tools, which provide different ways of learning
          depending on the developer’s preference. This combination of well-structured documentation
          and supporting resources makes Laravel one of the best frameworks for PHP developers, and
          a great model for how technical documentation should be designed.
        </p>
      </div>

      <div
        class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 lg:col-span-3"
      >
        <h3 class="text-xl font-semibold text-indigo-600 mb-3">
          5. Explain, in a couple of paragraphs, what you think are two major challenges around DNS
          configuration for less-technical customers hosting websites.
        </h3>
        <div class="text-gray-700 leading-relaxed text-sm space-y-3">
          <p>
            In my experience, two major challenges around DNS configuration for less-technical
            customers are understanding how DNS works in general and dealing with DNS caching. Many
            customers struggle with the concept that a URL like https://accounting.pco is
            essentially mapped to an IP address such as 192.0.0.1. The distinction between a
            human-friendly domain name and the underlying server address can be confusing, and this
            often leads to misunderstandings when something goes wrong with a site.
          </p>
          <br />
          <p>
            Another common issue is DNS caching. When changes are made to DNS records, users often
            expect them to take effect immediately, but because of caching at both the browser and
            global DNS level, updates can take time to propagate. This delay frequently causes
            confusion and frustration, as users may still see an outdated version of their site or
            believe something is broken on their end.
          </p>
        </div>
      </div>

      <div
        class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 lg:col-span-3"
      >
        <h3 class="text-xl font-semibold text-indigo-600 mb-3">
          6. A customer writes in to Support saying simply that their “site won’t build”. You have
          access to their build logs, and there you see this error: Build failed due to a user
          error: Build script returned non-zero exit code: 2. You have no more information than this
          and the site’s source repository is private so you cannot test the build yourself. How
          would you troubleshoot this issue? What steps would you take? Also, please compose your
          best customer-facing first response.
        </h3>
        <p class="text-gray-700 leading-relaxed text-sm mb-3">
          Since I’ve encountered a similar issue myself (when I first tried deploying a Laravel
          application without realizing it wasn’t fully supported on Netlify), I know how confusing
          a vague error like “exit code 2” can be. In cases like this, where the logs don’t provide
          enough detail, my first step would be to gather more information directly from the
          customer. Specifically, I’d ask about their setup, the framework they’re using, their
          build command, publish directory, and whether the project builds successfully on their
          local machine. From there, I can narrow down whether the issue is related to
          configuration, dependencies, or environment variables.
        </p>
        <br />
        <div class="border border-green-300 bg-green-50 p-4 rounded-lg">
          <h4 class="font-bold text-green-800 mb-1">Customer-Facing First Response:</h4>
          <p class="text-gray-800 whitespace-pre-line text-sm">
            Hi [Customer Name], Thanks for reaching out! I had a look at your build logs, and I can
            see that the build is failing with an exit code of 2. This typically means something
            went wrong during the build process, but the logs don’t provide enough detail to
            pinpoint the exact cause. To help troubleshoot, could you share a bit more about your
            setup? For example: Which framework or tool you’re using (Vue, React, Next.js, etc.) The
            build command and publish directory you’ve configured in your Netlify settings Whether
            the site builds successfully on your local machine using the same command In the
            meantime, you might also want to double-check that all required dependencies are listed
            in your project’s configuration and that any necessary environment variables are set in
            your Netlify dashboard. Once I have this information, I’ll be able to guide you more
            precisely toward a solution. Looking forward to helping you get this sorted out! Best
            regards, Kiyo
          </p>
        </div>
      </div>

      <div
        class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 lg:col-span-3"
      >
        <h3 class="text-xl font-semibold text-indigo-600 mb-3">
          7. How would you set up an http 301 status redirect from “/netlify/anything” on your site,
          to https://www.google.com/search?q=anything. Please provide the redirect formatting here.
          Now, how about a proxy redirect? Please add that proxy redirect rule directly to your
          site!
        </h3>
        For this scenario, I’d use Netlify’s _redirects file approach. Inside the _redirects file, I
        would add the following rule: "/netlify/:anything https://www.google.com/search?q=:anything
        301" This ensures that any request to /netlify/anything is permanently redirected with a 301
        status to Google’s search with anything as the query parameter.
        <h4 class="font-bold mb-1">HTTP 301 Redirect:</h4>
        <pre class="bg-gray-100 p-2 rounded text-sm overflow-auto text-red-600">
  "/netlify/:anything https://www.google.com/search?q=:anything 301"</pre
        >
        <p class="text-gray-700 leading-relaxed text-sm">
          That said, from a developer’s perspective, if I were working inside a framework with
          centralized routing (like Laravel, Vue Router, or Express), I might choose to manage these
          redirects in the routing configuration file. This way, it keeps all route logic in one
          place and makes it easier for the team to find and maintain later.
        </p>
      </div>

      <div
        class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 lg:col-span-3"
      >
        <h3 class="text-xl font-semibold text-indigo-600 mb-3">
          8. Please attempt to deploy a function on our service. This need not be complicated. It
          could be "Hello World". Note that failure to deploy is not failing the exercise! Whether
          you have trouble or not, please describe what you experienced and how you attempted to
          troubleshoot any issues you encountered.
        </h3>
        <p class="text-gray-700 leading-relaxed text-sm">
          I’m not entirely sure if I set it up perfectly, but I followed the Netlify documentation
          for creating a function. I installed the @netlify/functions package, then created a
          netlify/functions folder with a hello.js file that returns a simple greetings response.
          After that, I deployed it to my application. The function deployed successfully, and I was
          able to confirm that it was accessible via the .netlify/functions/hello endpoint.
        </p>
      </div>

      <div
        class="bg-white p-6 rounded-xl shadow-lg hover:shadow-xl transition duration-300 lg:col-span-3"
      >
        <h3 class="text-xl font-semibold text-indigo-600 mb-3">
          9. We understand you don't know anything about our internal procedures at this stage, but
          we want you to explain at a high level how you'd react to this situation: You receive a
          report of a severe security issue on www.netlify.com. You can't immediately confirm the
          report, so what steps might you take to investigate or substantiate the report? What might
          you say to the reporter, even though we haven't confirmed their assertion yet, that will
          instill confidence that our business is very concerned about security? You believe there
          is a reasonable chance the report is correct and the problem is very large and impactful.
          How might you escalate?
        </h3>
        <p class="text-gray-700 leading-relaxed text-sm">
          If I received a severe security report, I’d first review the details and attempt to
          validate the issue in a safe environment. At the same time, I’d immediately escalate it to
          the security/engineering team to ensure quick action. I’d also acknowledge the reporter
          promptly, thank them, and reassure them that we treat security concerns with urgency and
          are actively investigating.
        </p>
      </div>
    </div>
  </div>
</template>
