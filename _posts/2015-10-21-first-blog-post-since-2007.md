---
layout: post
---

So, I finally ditched my old website. Maintaining your own website is hard when
your job is to maintain websites/web services/tweetybirds of others. Anyway, my good ol' vim powered website
got replaced by [Jekyll](https://jekyllrb.com/). It's still vim powered, but Ruby generated. Ruby, yay. Continuous deployment, yay.
As if I would deploy a new blog post every day.

Anyways, I'll post something useful as it's my first blog post since 2007 or so. Here's a copy'n'paste solution
to [Project Euler's problem number 55](https://projecteuler.net/problem=55):

{% highlight python linenos %}
def lychrel(number):
    for i in range(51):
        number += int(str(number)[::-1]);
        if(number == int(str(number)[::-1])):
            return False;
    return True

def main():
    print sum(lychrel(num) for num in xrange(10, 10000));

if __name__ == "__main__":
    main()
{% endhighlight %}

That's about it. I'll try to come up with something clever for my next blog post. This is just a proof-of-concept really.
