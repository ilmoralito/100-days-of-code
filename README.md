# 100-days-of-code
#100DaysOfCode

#day 0 26-04-2020

Today I start my 100 days of code, it has not been easy, it has been a complex day but thank God here is the first day. Now I learned about Pre-rendering and Data Fetching in nextjs, specifically getStaticProps Details, I have a couple of doubts, first. How should I make more than one request for data using getStaticProps and second how do I assign the value to data props obtained as promises? I hope to answer this tomorrow and comment it here

#day 1 27-04-2020

Yesterday I was left with two doubts, first how to make more than one data request in the context of getStaticProps, and the second how to pass data obtained asynchronously to the props object that returns getStaticProps. On the first question right now I am making n requests to different resources using different files in the / lib directory. On the second doubt I have solved following examples presented by nextjs where the promise that returns an asynchronous function I put await before the answer to extract the data that then pass to props, the latter is possible because getStaticProps is an asynchronous function.

I have pending learning about getStaticPaths and getServerSideProps but as I have documented they are related to dynamic routes, so I will first refresh on the topic of dynamic routes

Today my son is 1.6 months old

#day 2 28-04-2020

Today I managed to understand how the dynamic routes workflow works in nextjs, I also think I improve the name of the commits so that when I read them I know what the issue was that day

#day 3 29-04-2020

Today I managed to understand the basic of Api Routes. Next day I am planing to implementa more real world example using Api Routes

#day 4 30-04-2020

Today i have been getting acquainted with next js dynamic api routes. What was planned on day 3 is pending

#day 5 01-05-2020

Today I recap about dynamic api routes using REST api. Tomorrow I plan to understand how to keep a state between pages

#day 6 02-05-2020 

Now I have taken my first steps in understanding how to handle common states between pages. Thanks to the excellent article https://reacttricks.com/sharing-global-data-in-next-with-custom-app-and-usecontext-hook/

#day 7 03-05-2020

#day 8 04-05-2020

I lost a bit of the north now, I try to understand the logic of the code of obtaining static data explained in the publication https://www.netlify.com/blog/2020/05/04/building-a-markdown-blog-with-next -9.3-and-netlify /? Utm_source = github & utm_medium = blog-cs & utm_campaign = devex

Specifically this code
```
const posts = ((context) => {
  const keys = context.keys()
  const values = keys.map(context)

  const data = keys.map((key, index) => {
    let slug = key.replace(/^.*[\\\/]/, '').slice(0, -3)
    const value = values[index]
    const document = matter(value.default)
    return {
      frontmatter: document.data,
      markdownBody: document.content,
      slug,
    }
  })
  return data
})(require.context('../posts', true, /\.md$/))
```
#day 9 05-05-2020

Today I have only managed to review some concepts, which include pages, link and data fetching. I need to organize in order to understand what comes next

#day10 06-05-2020

It is time to put into practice what I have learned. So I am creating my own site

#day11 07-05-2020

Today, building my personal site I have continued putting into practice what I have studied in nextjs. Now create a switch that changes from light to dark mode along with other minor style changes

#day12 08-05-2020

Today I am working on implementing the main blog site

#day13 09-05-2020

Now and tried to integrate open graph meta tags and twitter cards to the post detail view. It works, but I have not been able to resolve to get the base url of the site to attach it to the image path I have defined. This in order to properly display the image on twitter

#day14 10-05-2020

Solved the pending of the previous day, but when trying to show an image in the twitter card I have not been successful. I hope to solve tomorrow

#day15 11-05-2020

Now as recent days it has not been easy to continue with the challenge. My twitter is blocked and I will not be able to report on that channel. But here I am still continuous. Here is my progress, this is the most recent commit of the day https://github.com/ilmoralito/my-site/commit/dece138e2b69b8362aa19d532074696932b20cb0

By the way my twitter account is blocked because I logged out and I don't remember my password. I tried to access n times and consequently they blocked me for identifying suspicious behavior

#day16 12-05-2020

Implementing contact form, practicing using formik and next/router
