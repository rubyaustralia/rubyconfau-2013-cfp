# Sinatra in SIX lines - How to do crazy stuff with Ruby

A fun code analysis.

``` ruby
%w.rack tilt INT TERM..map{|l|trap(l){$r.stop}rescue require l};puts "== Almost Sinatra/No Version has taken the stage on 4567 for development with backup from Webrick"
$n=Module.new{extend Rack;a,D,S,q=Builder.new,Object.method(:define_method),/@@ *([^\n]+)\n(((?!@@)[^\n]*\n)*)/m
%w[get post put delete].map{|m|D.(m){|u,&b|a.map(u){run->(e){[200,{"Content-Type"=>"text/html"},[a.instance_eval(&b)]]}}}}
Tilt.mappings.map{|k,v|D.(k){|n,*o|$t||=(h={};File.read(caller[0][/^[^:]+/]).scan(S){|a,b|h[a]=b};h);v[0].new(*o){n=="#{n}"?n:$t[n.to_s]}.render(a,o[0].try(:[],:locals)||{})}}
%w[set enable disable configure helpers use register].map{|m|D.(m){|*_,&b|b.try :[]}};END{Handler.get("webrick").run(a,Port:4567){|s|$r=s}}
%w[params session].map{|m|D.(m){q.send m}};a.use Session::Cookie;a.use Lock;D.(:before){|&b|a.use Rack::Config,&b};before{|e|q=Request.new e;q.params.dup.map{|k,v|params[k.to_sym]=v}}}
```

## Notes

This talk is super awesome.

## Konstantin Haase

As maintainer of Sinatra, Konstantin is an Open Source developer by heart. Ruby has become his language of choice since 2005. He regularly contributes to different widespread projects, like Rubinius, Rack, Travis, Rails and MRI.

In 2012, Konstantin received the Ruby Hero Award for his outstanding contributions to the community.

He now works full time at Travis CI.

![Profile picture](https://raw.github.com/rkh/proposals/master/headshots/lyon-edited.jpg)

- [My website](http://rkh.im)
- [My twitter](https://twitter.com/konstantinhaase)
- [Past talk slides](https://speakerdeck.com/u/rkh/p/message-in-a-bottle)
- [Past talk video](http://www.youtube.com/watch?v=NG8goJpbKk0)
