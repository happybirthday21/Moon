---
layout: post
title: Today is..
date: 2020-11-12
#excerpt: "someone's special birthday!"
#tags: [sample post, code, highlighting]
#comments: true
---

someone's special birthday! Someone who brightens up my world and always makes me smile! 🥰
From the very first you understood me so well that it felt like we knew each other for a long time! And maybe we did at the study halls, huh? :P It's a mysterious story but also interesting, sweet and romantic with you. I couldn't wait to talk to you when something exciting happened. I wasn't afraid of being imperfect. So I could share with you my childhood fantasies, the dreams I haven't reached and the embarrasing events of my life. You listened with so much care that I wanted to share more. You were my prince on a white horse, and I'd be your princess with Loch Ness Monster as a pet. And everything is the same now and will be.. Today you've been 7691 days in this world and I'm the most glad about it because I was there with you in 149 days of it: Just next to my amazing partner and boyfriend. And for celebrating your awsomeness in your 21st birthday I made this for you to wish you a very happy birthday: Paljon onnea! I love you! ❤️

~~~ ruby
module Jekyll
  class TagIndex < Page
    def initialize(site, base, dir, tag)
      @site = site
      @base = base
      @dir = dir
      @name = 'index.html'
      self.process(@name)
      self.read_yaml(File.join(base, '_layouts'), 'tag_index.html')
      self.data['tag'] = tag
      tag_title_prefix = site.config['tag_title_prefix'] || 'Tagged: '
      tag_title_suffix = site.config['tag_title_suffix'] || '&#8211;'
      self.data['title'] = "#{tag_title_prefix}#{tag}"
      self.data['description'] = "An archive of posts tagged #{tag}."
    end
  end
end
~~~
