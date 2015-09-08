```
~/⇾ yell YOUR_USER_ID
fetching articles starting with 0
fetching articles starting with 10
fetching articles starting with 20
fetching articles starting with 30
fetching articles starting with 40

Finished! Find in this directory:
- yelp.html, a hreview-formatted HTML version
- yelp.json: raw JSON data.
```

**Using this code is against the Yelp Terms of Service** because they prevent
users (in section 6B iii of their [terms of service](http://www.yelp.com/static?p=tos&country=US))
against:

> Use any robot, spider, site search/retrieval application, or other automated device, process or means to access, retrieve, scrape, or index any portion of the Service or any Site Content;

However, section 5C makes it very clear that users own their contributed content.

> As between you and Yelp, you own Your Content.

Given that copying-and-pasting ones content out of Yelp is rather inconvenient, in
order to make 5C a reality, this code breaks 6B iii. It's an unfortunate overlap of
code and law.

Yelp, for the most part, is doing a decent job - they publish reviews in
the **hReview** microformat, and have APIs. And it's great that their TOS
is fair in ownership to data. However, their APIs are for businesses,
not users, and their TOS is unfair in access to data.

## Running

Instead of `YOUR_YELP_USER_ID`, you should put your user id. Find this by going to Yelp,
and to your user page, and looking in the URL. It'll be like:

    http://www.yelp.com/user_details?userid=FDJLFJDSKL

That end bit - the random letters after the `=`, is your userid.

    npm install yell
    yell YOUR_YELP_USER_ID
    
Note, you may need to cd into the yell subdirectory, and prepend the yell command with node.

    cd  node_modules/yell
    node yell YOUR_YELP_USER_ID
