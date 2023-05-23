# Comparing `tmp/democracy-1.0.22.tar.gz` & `tmp/democracy-1.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "democracy-1.0.22.tar", last modified: Tue May 23 06:59:53 2023, max compression
+gzip compressed data, was "democracy-1.0.23.tar", last modified: Tue May 23 10:29:27 2023, max compression
```

## Comparing `democracy-1.0.22.tar` & `democracy-1.0.23.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-23 06:59:53.912177 democracy-1.0.22/
--rw-rw-r--   0 a         (1000) a         (1000)    40852 2023-05-23 06:59:53.912177 democracy-1.0.22/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)    40089 2023-05-23 06:53:15.000000 democracy-1.0.22/README.md
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-23 06:59:53.912177 democracy-1.0.22/democracy.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)    40852 2023-05-23 06:59:53.000000 democracy-1.0.22/democracy.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)      156 2023-05-23 06:59:53.000000 democracy-1.0.22/democracy.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-23 06:59:53.000000 democracy-1.0.22/democracy.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-23 06:59:53.000000 democracy-1.0.22/democracy.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)     5601 2023-05-23 06:57:25.000000 democracy-1.0.22/pyproject.toml
--rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-23 06:59:53.912177 democracy-1.0.22/setup.cfg
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-23 10:29:27.400241 democracy-1.0.23/
+-rw-rw-r--   0 a         (1000) a         (1000)    45838 2023-05-23 10:29:27.400241 democracy-1.0.23/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)    45075 2023-05-23 10:26:15.000000 democracy-1.0.23/README.md
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-05-23 10:29:27.396241 democracy-1.0.23/democracy.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)    45838 2023-05-23 10:29:27.000000 democracy-1.0.23/democracy.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)      156 2023-05-23 10:29:27.000000 democracy-1.0.23/democracy.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-23 10:29:27.000000 democracy-1.0.23/democracy.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-23 10:29:27.000000 democracy-1.0.23/democracy.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)     5601 2023-05-23 10:28:49.000000 democracy-1.0.23/pyproject.toml
+-rw-rw-r--   0 a         (1000) a         (1000)       38 2023-05-23 10:29:27.400241 democracy-1.0.23/setup.cfg
```

### Comparing `democracy-1.0.22/PKG-INFO` & `democracy-1.0.23/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,158 +1,199 @@
-Metadata-Version: 2.1
-Name: democracy
-Version: 1.0.22
-Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
-Author-email: Gregory Cohen <gregorycohen2@gmail.com>
-Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
-Project-URL: Homepage, https://github.com/gregoryc/democracy
-Keywords: ai,empowerment,agi,agis
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.0
-Description-Content-Type: text/markdown
-
-                      Practical self-empowerment utilities  
-                          covering every facet of life  
-  
+<h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life</h1>  
 These tools are for everyone  
   
-It doesn't matter what political ideology you favor, these tools are all still  
-very valuable. You can live in Canada, the US, Russia, China or Africa, it  
-doesn't matter.  
+It doesn't matter what political ideology you favor, these tools are all  
+still very valuable.  
+You can live in Canada, the US, Russia, China or Africa, it doesn't matter.  
   
 I intend to make people more able.  
-     __________________________________________________________________  
   
-   This lists all of the programs. Youtube channel here Democracy  
+   This lists all of the programs. Youtube channel here [1] Democracy  
    YouTube Channel (youtube.com/gregorycohen1) and  
-   facebook.com/democracygregoryc  
+   [2] facebook.com/democracygregoryc  
   
-                         Most important software here:  
+Most important software here  
   
    Music program (Crystal and Ruby), see fix_the_society folder  
   
    Ultimate chat app (Win, Lin, CLI)  
   
    Discourse Generator Program vesion 1 and version 2 (node, ruby, browser  
    (kind of like Siri); and C++ STL)  
   
    And Semantic metadata project  
   
    And “Emerald C” (the “Best Programming Language”)  
-  
    There is also a desktop widget for that site, and old random sentence  
    generator (useless) and an old compiler for my own programming  
-   language. Those aside, there are these 91 programs  
+   language. Those aside, there are these 93 programs  
   
- All of these programs are mostly self-contained. This is a really good thing.  
+All of these programs are mostly self-contained. This is a really good thing.  
   
-                            Few or no dependencies!  
+Few or no dependencies!  
   
-   My email is gregorycohen2@gmail.com and I really would like to make  
+   My email is [3] gregorycohen2@gmail.com and I really would like to make  
    open source software. Everything I have is BSD licensed.  
    If this software gets you a job or makes you money or improves your  
-   life or makes things easier for you, please consider donating. I have  
-   released this software under the BSD license (a very liberal license)  
-   for everyone to use and modify. I would appreciate it greatly if some  
-   people could return the favor :)  
-  
-   Democracy gem github Ruby Gem  
-     __________________________________________________________________  
-  
-           Without further ado, here are the 91 documented programs.  
-     __________________________________________________________________  
-  
-   ### Ultimate chat application (linux)  
-   ![Image](./images/1.png)  
-   The Linux version of this very useful tool.  
-   See also  
-   chat_rb (which is really, really useful, it could replace bash and  
-   ChatGPT)  
-     __________________________________________________________________  
+   life or  
+   makes things easier for you, please consider donating. I have released  
+   this software under the BSD license (a very liberal license) for  
+   everyone to use and modify.  
+   I would appreciate it greatly if some people could return the favor 🙂  
+  
+   https://github.com/gregoryc/democracy  
+  
+   HOW TO DOWNLOAD/INSTALL  
+  
+   gem unpack democracy  
+  
+   gem install democracy  
+  
+   work to download or install  
+  
+   pip install democracy  
+  
+   or  
+  
+   pip3 install democracy  
+  
+   works for pip  
+  
+   git clone https://github.com/gregoryc/democracy  
+  
+   works for github  
+  
+   Important because python is very popular  
+     * [4] https://pypi.org/project/democracy  
+  
+   Any Python “dweeb” (AI person who doesn't value personal dynamism)  
+   searching  
+   for “democracy”--for example--BECAUSE THEY ARE A RATIONAL HUMAN BEING  
+   AND CARE ABOUT PEOPLE, would find this,  
+   probably as the first result.  
+  
+   How many options are there? 37 projects for “democracy”  
+  
+   Almost nothing.  
+  
+   ONLY MY PROJECT IS CALLED “DEMOCRACY.” SAME ON RUBYGEMS FOR RUBY.  
+  
+   On rubygems, there are even fewer results. MY CODE WILL BE FOUND.  
   
-   ### Ultimate chat application.exe  
-   ![Image](./images/2.png)  
+   I shared my gem on the rubytalk forum, and maybe other forums. I have a  
+   youtube channel. I have a facebook.  
+     * [5] https://www.rubygems.org/gem/democracy  
+     * [6] https://www.linkedin.com/in/gregory-cohen-274333261/  
+     * [7] https://www.youtube.com/GregoryCohen1  
+     * [8] https://facebook.com/democracygregoryc  
+  
+   Gems that link to this gem on RubyGems  
+     * [9] https://www.rubygems.org/gems/computers  
+     * [10] https://www.rubygems.org/gems/democracy  
+     * [11] https://www.rubygems.org/gems/linux  
+     * [12] https://www.rubygems.org/gems/string  
+     * [13] https://www.rubygems.org/gems/unix  
+  
+   There are only 3 results on rubygems that are not by me, if one  
+   searches “democracy”  
+  
+   So I will leave a legacy.  
+  
+   And I will be found by AIs, assuming they continue to exist.  
+  
+   [14] Democracy gem github      [15] Ruby Gem      [16] Python PIP Package  
+  
+Without further ado, here are the 93 documented programs.  
+  
+   ### Ultimate Chat Application  
+  
+   ![UCA](./images/2.png)  
    Windows version of Ultimate Chat Application.  
    There is so much potential with this program.  
    This is a non-AI chatbot. It's not based on generative AI or AI of any  
    sort.  
    It is self-explanatory, it tries to give a better answer.  
    Still a work in progress.  
    Source code is in PP.rb  
    Generates a hyper optimized C program that is able to respond to  
    prompts locally as fast as theoretically possible using switch  
    statements  
-     __________________________________________________________________  
+   ### Discourse Generator  
+  
+   The use of Javascript (and possible Ruby) to create a Javascript  
+   library (and perhaps a Chrome extension and perhaps a command line tool  
+   and perhaps a GTK or QT program) that helps people (by using textboxes  
+   or command line prompts) to create high quality communications, would  
+   be wonderful. Think of how poor quality responses to communications can  
+   be. If someone created one or more tools that could be easily added on  
+   web pages, that would augment someone's life to help create goal and  
+   value oriented responses (or original communications), then there is  
+   literally nothing that couldn't solve. This might be the most useful  
+   library ever created. There could be a tool that would help with  
+   democracy. Human being + augmentive tool = civil discourse, eventually  
+   resulting in liberty. This would enable democracy to work. Imagine if  
+   50% of all websites used this library. This would help people to be  
+   goal or value oriented, and not be coming up with terrible  
+   communications that, for example, insult people's mothers or education.  
+   ### Replace Not In Place  
   
-   ### Replace not in place  
    This is like gsub, but for strings, not for regular expressions  
    See also  
-   gsub  
-     __________________________________________________________________  
+        gsub  
+   ### Generate Do More  
   
-   ### Generate do more  
    Generate the job search program from the inspect program.  
    See also  
-   inspect  
+        inspect  
    job search, job search, etc.  
-     __________________________________________________________________  
+   ### Replace In Place  
   
-   ### Replace in place  
    replace_in_place tool replaces a string, not a regular expression, with  
    another string  
    Example  
    replace_in_place cat dog file  
-     __________________________________________________________________  
-  
    ### Emerald browser  
-   ![Image](./images/S1.png)  
-   ![Image](./images/S4.png)  
+  
+   ![UCA](./images/S1.png)  
+   ![UCA](./images/S4.png)  
    Emerald browser is a really powerful new browser  
    See README  
    It works based on panes.  
    Read the documentation for “open”, “close” and also the README file.  
-     __________________________________________________________________  
+   ### Job Search  
   
-   ### Job search.exe  
    job search is a work in progress, but it works, and it helps you to  
    progress, in life  
    job search automatically generates resumes and cover letters for all of  
    the jobs that you could have.  
    COVID makes life hard.  
    People are unemployed, etc.  
    People could have more jobs.  
-   job search is a graphical, cross platform program (generated from the  
+   Job search is a graphical, cross platform program (generated from the  
    inspect_list program) that generates and downloads dynamic PDFs of  
    Resumes and Cover Letters that are tailored for each and every possible  
-   job that you could apply for on Indeed. It is very freaking  
-   practical!!!!!!!!!!!!!!!!!!!!!  
+   job that you could apply for on Indeed. It is very freaking practical!  
    First, you need to click on the bottom part of it. It copies that code  
    into your browser. Then you right click on a browser page and go to  
    “Inspect” (the same can be done by doing Control + F12). Make sure you  
    are on Indeed.  
-   Search for something on Indeed, like “labourer”.  
+   Search for something on Indeed, like “labourer.”  
    For each result, a new resume and cover letter will be downloaded, each  
    of which is geared for that specific job positing, with the company  
    name and copy role in both of them  
    This way, you can show employers that you really care!  
    The script will open up later pages on Indeed as well.  
    You can generate hundreds of resumes and cover letters as well  
    HTML documents will be downloaded.  
    You have to convert them to PDF, which chrome can do by doing  
    --print-to-pdf  
    Or you can do it manually  
-   (On Windows, you can use Cygwin and do this )  
+   (On Windows, you can use Cygwin and do this)  
    (You need to be in the Downloads folder)  
-   (Find it by doing “cd ”, “cd ..”, etc. )  
+   (Find it by doing “cd [folder]”, “cd ..”, etc. )  
    for i in Downloads/*; do ./chrome --headless --print-to-pdf-no-header  
    “$i” --print-to-pdf=“$i.pdf”; done  
    Then you have to click on the second part, and run that in your command  
    prompt or terminal (Windows or macOS or Linux)  
    All of the generated resumes are numbered, starting from what you  
    enter, which is probably 0  
    They would look like 0_Business_Job.html  
@@ -187,104 +228,242 @@
    Count on this program, because it is here to serve all of humanity.  
    This program can help fix unemployment problems of an economy, in a  
    nonpartisan way.  
    Have you ever thought, that people don't look for work, because it is  
    hard?  
    People can work 2 or 3 jobs  
    See also  
-   find_housing  
+        find_housing  
    to_buy  
-     __________________________________________________________________  
+   ### Gsub In Place  
   
-   ### Gsub in place  
    gsub_in_place is like gsub, which replaces all instances of a regular  
    expression globally  
-     => result  
+   [regular expression 1] [regular expression 2] => result  
    Example  
    gsub_in_place . FOO file  
    Would make all characters in “file” become “FOO”.  
    gsub_in_place cat dog file  
    Would make all instances of “cat” “dog”  
    It is much cleaner than “sed”.  
    You don't need to have “sed” installed to run this program.  
    It doesn't read from the standard input  
    It takes exactly 3 arguments, no more, no fewer.  
-   See Also  
-   gsub  
-     __________________________________________________________________  
+   See also  
+        gsub  
+   ### Find Housing  
   
-   ### Find housing  
    This is a nice tool to find housing with! Everyone needs housing. This  
    can help with that.  
    It is a nice, simple command line tool. You enter the minimum and  
    maximum prices, and Kijiji opens with your options.  
    Along with the resume program, these tools can be __VERY PRACTICAL__  
    for daily things.  
-   World War III might be scary, but if you maximize daily things you can  
-   be fine.  
    See also  
-   to_buy  
-     __________________________________________________________________  
+        to_buy  
+   ### Faster Rhyme  
+  
+   Enter basename to make songs folder in (folder/songs, num songs =  
+   13000)  
+   Usage faster_rhyme [folder] (processes files "1.json" and "21.json" by  
+   default)  
+   Example output of a song  
+   -----------------------------------------------------------------------  
+   -----  
+   (NO COPYRIGHT RESTRICTIONS ON THIS CONTENT WHATSOEVER. FULLY PUBLIC  
+   DOMAIN)  
+   Name the song or poem as you wish, resell it, but please positively  
+   influence culture  
+   Subject matter | Category 1 -- Abuse of philosophical universalism  
+   (making  
+   broad claims while intentionally not trying to understand things or see  
+   any sides of anything whatsoever, childish behavior worse  
+   than a 3 year old, acting retarded)  
+   VERSE  
+   Brittle as possible, they are truly unguarded  
+   Any novelty, they have disregarded  
+   Their remissness is spectacular, the world they've bombarded  
+   The clique is so insular, I swear they're retarded  
+   Enlightenment values, they have not safeguarded  
+   Any novel ideas, they automatically have discarded  
+   Maybe the rebels and true communicators are off the grid  
+   Lack of thought makes an grown-up the absolute worst kid  
+   Can we stop this, their non sense they overdid  
+   What horrendous non sense these creeps did  
+   Tunnel vision, everyone and everything they forbid  
+   They're such failures, themselves they outdid  
+   CHORUS  
+   They're such failures, themselves they outdid  
+   Cutting out the conversation, putting on the lid  
+   Don't have to do with ego or id  
+   Running away from conversation just like a kid  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   They don't have decency, they automatically disregard  
+   Having an open mind, should not be so hard  
+   They don't care about anyone, don't need no bodyguard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They're a complete failure, they only neglect  
+   This is plain, anyone can detect  
+   They don't care about pain or the past, they don't want to recollect  
+   This needs to be called out, one should be direct  
+   They want man lower, lower just as if an insect  
+   VERSE  
+   Thinking itself resides in their territory of circumvention  
+   Complete neglect, complete inattention  
+   They have no genuine intention  
+   We need change, we need intervention  
+   Violence is second nature to them, their friends they've bombarded  
+   Any novel ideas, they automatically have discarded  
+   The clique is so insular, I swear they're retarded  
+   Any novelty, they have disregarded  
+   Any novelty, they have disregarded  
+   Brittle as possible, they are truly unguarded  
+   The clique is so insular, I swear they're retarded  
+   Any novel ideas, they automatically have discarded  
+   Enlightenment values, they have not safeguarded  
+   Their remissness is spectacular, the world they've bombarded  
+   They don't care about your feelings, they don't regard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They don't have decency, they automatically disregard  
+   Working don't matter for this, whether day or graveyard  
+   CHORUS  
+   They're such failures, themselves they outdid  
+   Cutting out the conversation, putting on the lid  
+   Don't have to do with ego or id  
+   Running away from conversation just like a kid  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   They don't have decency, they automatically disregard  
+   Having an open mind, should not be so hard  
+   They don't care about anyone, don't need no bodyguard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They're a complete failure, they only neglect  
+   This is plain, anyone can detect  
+   They don't care about pain or the past, they don't want to recollect  
+   This needs to be called out, one should be direct  
+   They want man lower, lower just as if an insect  
+   VERSE  
+   The truth is what they wish to disregard  
+   Their behavior is garbage, it should be thrown in the junkyard  
+   They act like a retard  
+   Behaving just like in the schoolyard  
+   In their ivory tower, with the castle and guard  
+   Their behavior makes them charred  
+   Thinking differently shouldn't have to be hard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   Working don't matter for this, whether day or graveyard  
+   They don't care about your feelings, they don't regard  
+   They are failures, down at the boulevard  
+   They don't have decency, they automatically disregard  
+   They're a complete failure, they only neglect  
+   They don't speak the language of the people or their dialect  
+   This is not right, this is completely incorrect  
+   The only focus on “responses”, they just want to deflect  
+   The lies are put forth, the lies they erect  
+   CHORUS  
+   They're such failures, themselves they outdid  
+   Cutting out the conversation, putting on the lid  
+   Don't have to do with ego or id  
+   Running away from conversation just like a kid  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   They don't have decency, they automatically disregard  
+   Having an open mind, should not be so hard  
+   They don't care about anyone, don't need no bodyguard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They're a complete failure, they only neglect  
+   This is plain, anyone can detect  
+   They don't care about pain or the past, they don't want to recollect  
+   This needs to be called out, one should be direct  
+   They want man lower, lower just as if an insect  
+   VERSE  
+   They don't have decency, they automatically disregard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They want the status quo, it's all they crave  
+   The speeches of the past, they only wish to engrave  
+   They act as bad as possible, they don't know how to behave  
+   Their sucked in their circle, they never wave  
+   Away from the truth, on the outskirt  
+   With pre-thought of ideas, they automatically assert  
+   Any progress is fleeting with them, they revert  
+   Disingenuous to the extreme, the society they subvert  
+   The society is the ones who hurt  
+   ---  
+   ### Inspect List  
   
-   ### Inspect list  
    This tool is really powerful  
-   In an abstract world, there are lists of things   
-   There can be lists that contain other lists , ]  
+   In an abstract world, there are lists of things [1, 2, 3]  
+   There can be lists that contain other lists [[1, 2], [3, 4]]  
    This tool by inspecting a list  
    Does  
    * Generates HTML from the list, with divs and spans  
    You can then visually view that list.  
    Or you can use the HTML for something else  
    * Generates a GTK program for Windows and Linux, where that list is  
    converted into widgets  
    You are “inspecting” the list and turning it into other representations  
    A resultant c_program is created for both Windows and Linux. You need  
    to have MXE installed on a UNIX-like system to make it work (e.g.,  
    Linux)  
    The Job Search program was created by using this program!  
    You could make an entire website with that program from the command  
    line  
-   inspect   
+   inspect [File.read(“page”)]  
    cat list | args inspect  
    also would work  
    (See “args”)  
    See also  
-   args  
+        args  
    job search  
    The usage of this program is like this  
-   inspect , ]  
-     __________________________________________________________________  
+   inspect [[“Hi there”, “This is text”], [200, “Man”, 3.6]]  
+   ### Google Speak  
   
-   ### Google speak  
    Google speak is really useful. It speaks a statement using the Google  
    Translate voice, which is probably the most authoritative and  
    high-quality text-to-speech voice that exists.  
    It's kind of like “espeak” or similar tools, but it is much better.  
    You need an internet connection for it to work.  
    It is probably limited at 100 characters.  
    There is a “singing program”, not really a tool, in this software  
    project that gets around that.  
    TODO  
    Make the alarm clock program in this software project use this voice.  
    It is quite reliable.  
    It is probably “unlimited”.  
    I haven't had Google block me from using it ever.  
    Which is a good thing.  
-     __________________________________________________________________  
+   ### Make Server  
   
-   ### Make server  
    make_server is powerful.  
    make_server takes expressions, either Javascript or C++, and generates  
    a resultant program from that.  
    The Javascript mode currently doesn't work.  
    Not only is a program made, the resultant program is an entire  
    webserver, that uses FastCGI to run really fast code.  
    The arguments work in an interesting way.  
-   make_server      
-    ...  
+   make_server [function_name] [iterable] [condition, it can be “true” to  
+   do the following argument always] [code list separated by semicolons,  
+   the last statement is an expression, and is returned by the function]  
+   [function_name2] ...  
    You have to give 4 arguments every time.  
    There was an “otherwise” mode as an “else”, but I don't think that's a  
    part of the program anymore.  
    It doesn't need to be.  
    You have to give 4 arguments for each function.  
    So you can do  
    make_server 4args 4args 4args 4args  
@@ -356,43 +535,40 @@
    You don't have to sacrifice on those things.  
    Contributions on this program would be really appreciated.  
    It is called “make_server” for now.  
    There was also a mode to generate javascript.  
    I have to make that work again.  
    The entire program is just one file.  
    My email is gregorycohen2@gmail.com  
-     __________________________________________________________________  
-  
    ### Selectlines  
+  
    selectlines shows all nonblank lines from the input  
    Example  
    cat file | selectlines  
    (echo 2; echo; echo; echo) | selectlines  
    => 2  
    The result would be 2, with no blank lines after that  
-     __________________________________________________________________  
-  
    ### Communicate  
+  
    Communicate is cool.  
    Communicate runs a Ruby expression after speaking a prompt (the first  
    argument) and getting your verbal answer (using something unfortunately  
    called “nerd-dictation”, which is a wrapper around another program  
    which deals with speech recognition)  
    Communicate allows you to have conversations with your computer, and it  
    is cross platform  
    (Or it hopefully is)  
    communicate 'What is the best color?' 'case text; when /blue/; puts  
    “You are right!”; when /red/; puts “Red is a bad color”; end '  
    That would be an example of how one could use “communicate”  
    Make sure you have nerd-dictation on your computer  
    The name nerd-dictation is absolutely awful, and I have to criticize  
    him for not making it have a better name, but it works.  
-     __________________________________________________________________  
+   ### Super Trans  
   
-   ### Super trans  
    super_trans is an offline translation program  
    It uses “Apertium”, which can do offline translation.  
    You can do translation anywhere with it.  
    It generates a webpage from the input text that not only has all  
    language translations embedded in it, it dynamically adjusts the  
    website page content to the web browser's “current language”.  
    You need to have a folder called “translation_folder” in your home  
@@ -403,55 +579,47 @@
    This is really powerful.  
    Some notes  
    This is worse than t.js in this software project  
    The resultant HTML is really big. It is too big.  
    “Automatic translation” is really powerful.  
    This translates into literally dozens of languages.  
    See also  
-   t.js  
-     __________________________________________________________________  
+        t.js  
+   ### To Buy Old  
   
-   ### To buy old  
    Old to buy tool, not that good  
-     __________________________________________________________________  
-  
    ### Executable  
-   Makes all the files in the current directory executable  
-     __________________________________________________________________  
   
+   Makes all the files in the current directory executable  
    ### Questions  
+  
    This program allows you to communicate with all important people in  
-   youife cycically and very easily. It's much easier than texting or  
+   your life cycically and very easily. It's much easier than texting or  
    normal emailing.  
+   It uses “email”, which currently doesn't work for Gmail.  
    See youtube.com/GregoryCohen1  
    See also  
-   tb (to buy)  
+        tb (to buy)  
    The youtube documentation video  
-     __________________________________________________________________  
-  
    ### Underline  
-   Underlines text  
-     __________________________________________________________________  
   
+   Underlines text  
    ### Processes  
+  
    Processes lists all processes with a certain name  
    For example  
    processes sh  
    processes bash  
    processes ruby  
    processes gsub  
-     __________________________________________________________________  
-  
    ### Emeraldc  
-   # EmeraldC  
+  
    The Ultimate C Preprocessor  
    I'm naming this preprocessor “Emerald C.”  
-   https://cboard.cprogramming.com/c-programming/181160-hi-i-have-created-  
-   some-work-i-think-will-really-valuable-community.html?s=589b5504cd0e3c2  
-   dc90e9abd8b66906f  
+   [17] Link  
    Howdy!  
    First, let me state that I am very much a perfectionist.  
    C is a wonderful language. C is probably the perfect programming  
    language. It is one of the top two most widely used languages for a  
    reason.  
    Now, there are some problems with it of course, but it's hard to think  
    of a more elegant language than it.  
@@ -465,27 +633,23 @@
    make another language. As a result, there are thousands of different  
    languages.  
    Well, recently, I made a preprocessor for C, that makes C incredibly  
    EASY.  
    C is fast and straightforward without it, but it has many features.  
    If one runs the command line preprocessor, with the “--features” flag,  
    the program shows all of its features  
-   --------------------------  
-  
-  A Better C  
-  
-   --------------------------  
+   A Better C  
    C is a fantastic language. C compiles insanely fast, is the fastest  
    language there is, is very clear, is native to all systems, and is  
    useful for all purposes.  
-   Some people, e.g., Bjarne Stroustrup, consider that C is "not good  
-   enough", and make languages like C++ or D (or thousands of others)  
+   Some people, e.g., Bjarne Stroustrup, consider that C is “not good  
+   enough”, and make languages like C++ or D (or thousands of others)  
    This is not necessary.  
-   There is no reason to use Python instead of C for "simple scripting  
-   tasks"  
+   There is no reason to use Python instead of C for “simple scripting  
+   tasks”  
    Some functions can be used as methods  
    Makes for an excellent “scripting language” (which is really just  
    native C without things making it slow)  
    1 String Interpolation “String interplation like this #{foo} ” Calls  
    the join() function (talked about below to join strings,  
    delim is a static global in each module called “sep”.  
    Make sure you free() the string after. The string is stored in a static  
@@ -501,17 +665,17 @@
    The preprocessor detects if you use and adds -lpcre2-8 to the link  
    flags if you use it. Use $" for substitutions in argument 3 gsub(a, b,  
    c)  
    8 join Joins an array of strings, to split(), use C's strtok (very  
    fast)  
    9 Lightweight regexes are added, almost 15 times as fast as C's built  
    in regex. They are very simple, they only have bracket expressions,  
-   like .  
+   like [a-z].  
    To use it, you need to pass a buffer of the size of the expansion of  
-   the regex. Foo would be Foo. That would be stored  
+   the regex. Foo[a-fA-F] would be Foo[abcdefABCDEF]. That would be stored  
    in a buffer.  
    From testing, 15x times faster than C's regex POST COMPILATION, if  
    compilation keeps happening, it might be hundreds of times faster.  
    Uses static inline functions, NO HEAP MEMORY unless you malloc  
    before().  
    10 print Like old python print “Hello” (fputs);  
    11 print_int prints a number and returns the number, can be chained  
@@ -524,21 +688,20 @@
    (frees str, sets to NULL, and frees other recent stuff)  
    asprintf() is another useful function which is UNIX-centric.  
    open_memstream() could be an alternative to std::string.  
    It works very well with each_line or by_lines (see above)  
    These features seem simple, but they can make C programming much, MUCH  
    easier  
    for example (insignificant example)  
-int main() {  
-    stdin.each_line { |line|  
-        print line;  
-    }  
-    free(line);  
-}  
-  
+   int main() {  
+   stdin.each_line { |line|  
+   print line;  
+   }  
+   free(line);  
+   }  
    You can iterate over the standard input like Ruby  
    The thing with this is that it has 100% speed. The resultant  
    preprocessed program becomes a normal C program  
    The compile and run time for a program (if you use tcc and not gcc) can  
    be about 24 milliseconds, which is faster than Ruby to run.  
    Even though the program is preprocessed, re-preprocessed, compiled,  
    assembled, linked, turned into an executable, and then run  
@@ -549,168 +712,148 @@
    else likes this work, and would like to use it, or to work with me.  
    Best regards,  
    Gregory  
    Current program is written in Crystal (crystal-lang.org) -- it was  
    written in ruby, it could be ported to another language.  
    I would like to make this self-hosting, but that would take a little  
    bit of work.  
-  
-About the Name  
-  
+   About the Name  
    Years ago, I really, really liked Compiz  
    Compiz then forked into Beryl. There was the Emerald Window Manager,  
    which was really nice and beautiful.  
    I actually made another programming language. I made 2 other  
    programming language. One was a full compiler and assembler, that ran  
    code in memory. It was around 16 thousand lines of code. I made a  
    programming language that had the syntax of Python or Ruby, but  
    transpiled into C++. I called that C += 2. I used that other language,  
-   and I created a Web Browser in it based on Chrome. I called it "Emerald  
-   Browser." Emeralds are beautiful green gems.  
-  
-   "Emerald is a gemstone and a variety of the mineral beryl colored green  
+   and I created a Web Browser in it based on Chrome. I called it “Emerald  
+   Browser.” Emeralds are beautiful green gems.  
+   “Emerald is a gemstone and a variety of the mineral beryl colored green  
    by trace amounts of chromium or sometimes vanadium. Beryl has a  
    hardness of 7.5–8 on the Mohs scale. Most emeralds are highly included,  
    so their toughness is classified as generally poor. Emerald is a  
-   cyclosilicate." --Wikipedia  
-  
+   cyclosilicate.”  
+   --Wikipedia  
    There was a browser with a terminal built in to it.  
    I show things off on my youtube channel, which I'm not going to link  
    here but is linked in my other repo.  
    This new language is better. It's ideal.  
-   ---  
    QUESTIONS  
-   ---  
    Why not use Rust?  
-$ time rustc a.rs  
-real    0m0.637s  
-user    0m0.502s  
-sys     0m0.160s  
-  
+   $ time rustc a.rs  
+   real 0m0.637s  
+   user 0m0.502s  
+   sys 0m0.160s  
    Rust takes 0.637 seconds to compile an empty file!  
    That is not ideal.  
-     __________________________________________________________________  
+   ### Last Nth  
   
-   ### Last nth  
    Last nth gets the last n lines from the standard input  
-     __________________________________________________________________  
-  
    ### Speakcat  
+  
    Speak cat is a tool like “cat”, which shows the content of files  
    (technically, it combines the content of files).  
    But speak cat also speaks the text.  
    Which could be useful in some circumstances.  
    It's kind of like “tee” to your ear.  
-     __________________________________________________________________  
+   ### Uca Cli  
   
-   ### Uca cli  
    CLI for uca app  
-     __________________________________________________________________  
+   ### Big Num  
   
-   ### Big num  
    big_num speaks really big numbers  
    Enter an expression, such as 2 ** 1000, and you'll see the result  
-     __________________________________________________________________  
-  
    ### Squeeze  
+  
    Squeeze is kind of like “sponge” from “moreutils”  
    But squeeze is different.  
    Squ  
    Squeeze reads all input, then it prints it back omitting argument 1  
    line from the front, and argument 2 lines from the back  
    Example  
    squeeze 1 1  
    This would omit the first line and the last line  
    squeeze 5 3  
    This would omit the first 5 lines and the last 3 lines  
-     __________________________________________________________________  
-  
    ### Foreach  
+  
    Reads a bunch of lines  
    Then a ruby expression is evaluated as the last line  
    The result is outputted in an argument.  
    You can enter /dev/null if you don't want an output file  
    “t” is better  
    See also  
-   t  
-     __________________________________________________________________  
-  
+        t  
    ### Dictate  
+  
    Dictate opens web pages in emerald browser, or in any browser  
    (depending on the environment variable set), by you speaking, instead  
    of typing.  
    There is a mode called c_mode, that allows you to make code from  
    speaking.  
-     __________________________________________________________________  
-  
    ### Prepend  
+  
    prepend prepends input taken from the standard input to a file  
    Usage  
-   prepend   
+   prepend [file]  
    This is text to be prepended  
-     __________________________________________________________________  
+   ### Chat Rb  
   
-   ### Chat rb  
    This program is excellent.  
    It's essentially a mix of ChatGPT and a shell, such as bash or ZSH.  
    It has a bunch of features.  
    It can display a file or change to a folder just by mentioning it.  
    It outputs chatgpt data to an output folder in home folder and copies  
    it to clipboard  
    To run a shell command, prefix things with “c”, such as c gcc.....  
-     __________________________________________________________________  
-  
    ### Undump  
+  
    undump is the opposite of dump  
    Example  
    echo cat | dump | undump  
    => cat  
    echo cat | dump  
    => “cat”  
    echo '“cat”' | undump  
    => cat  
-     __________________________________________________________________  
-  
    ### Append  
+  
    Appends text to file  
    Example  
    append file  
    This is more text to be appended  
-     __________________________________________________________________  
-  
    ### Email  
+  
+   ( This currently doesn't work for gmail since 2022 due to policy  
+   changes. :( )  
    A simple and practical tool to email people using Himalaya  
    Himalaya needs to be installed first  
    You would need to configure the script by changing its source code.  
    Modes  
-   email   
-   Email   
-   email   
+   email [no arguments]  
+   Email [yourself]  
+   email [addr]  
    Email one email address  
-   email     
+   email [Subject] [addr] [option more addrs]  
    Example  
    Email 'Gregory, I love your software!' gregorycohen2@gmail.com  
    my_friend@outlook.com person@example.com  
-     __________________________________________________________________  
-  
    ### Floor  
-   Gets the floor of numbers e.g. 21.3 -> 21  
-     __________________________________________________________________  
   
+   Gets the floor of numbers e.g. 21.3 -> 21  
    ### Query  
+  
    This is the top part of the job search, job search, etc. program for  
    Linux. The Linux program itself is called “linux_c_program”. The part  
    normally only works for Windows. This program works for Linux.  
-     __________________________________________________________________  
-  
    ### Lines  
-   Lines gets the number of files in the current folder that you are in.  
-     __________________________________________________________________  
   
+   Lines gets the number of files in the current folder that you are in.  
    ### Clock  
+  
    clock is useful  
    clock is a command line alarm clock  
    It wakes you up at 8:14, or at a time specified  
    Usage  
    clock  
    Runs clock  
    clock 15 30  
@@ -718,71 +861,37 @@
    clock 9 0  
    Sets an alarm clock for 9 in the morning  
    It uses flite to wake you up  
    It speaks with a bunch of voices  
    To stop it  
    Run this command  
    clock stop  
-     __________________________________________________________________  
-  
    ### Emoji  
+  
    Emoji converts words to emojis from the standard input  
    It can also speak the output  
    It can also copy the output to your clipboard  
    It is very useful  
-     __________________________________________________________________  
-  
    ### Close  
-   “Close” is a simple program that closes “Emerald Browser”, a new web  
-   browser based on the same engine as Chrome. Currently, Emerald Browser  
-   only works on Linux and Mac (Or Windows with Windows Subsystem for  
-   Linux or a Virtual Machine, but getting it to work might be tricky).  
-   “close” closes the Web Browser, which is normally full-screen.  
-   More accurately, it kills the browser, and all other copies of Emerald  
-   Browser.  
-   Since they are normally full screen, presumably the user would only  
-   have one instance of the browser open.  
-   The browser can have multiple panes (kind of like tabs) open, depending  
-   on how the browser is compiled.  
-   The browser can also be transparent, depending on how it is compiled.  
-   “Close” is supposed to be used in tandem with “open”, which is a  
-   command line tool to open the browser.  
-   open  ---->  gets searched in google, and then opened  
-   When you are done, you can do  
-   close  
-   Which closes the browser. It is a simple command.  
-   Currently, Emerald Browser is incomplete. A program exists in this  
-   software project that allows you to open up multiple browser tabs (one  
-   or more tabs) simply by speaking.  
-   Voice recognition would google the multiple sites that you say in your  
-   query (separated by “and”)  
-   “facebook and youtube and google”  
-   It's hard to get more direct than that!  
-   Emerald browser has a built in the top. The terminal is the navigation  
-   bar.  
-   Some more work needs to be put into the browser.  
-   Currently, new tabs can't be opened, which might be a dealbreaker for  
-   some people.  
-   Currently, content, like YouTube videos, can't be made fullscreen.  
-   If anyone wants to contribute, feel free to! :)  
-   “Close” is a simple program that closes “Emerald Browser”, a new web  
+  
+   “Close” is a simple program that closes “Emerald Browser,” a new web  
    browser based on the same engine as Chrome. Currently, Emerald Browser  
    only works on Linux and Mac (Or Windows with Windows Subsystem for  
    Linux or a Virtual Machine, but getting it to work might be tricky).  
    “close” closes the Web Browser, which is normally full-screen.  
    More accurately, it kills the browser, and all other copies of Emerald  
    Browser.  
    Since they are normally full screen, presumably the user would only  
    have one instance of the browser open.  
    The browser can have multiple panes (kind of like tabs) open, depending  
    on how the browser is compiled.  
    The browser can also be transparent, depending on how it is compiled.  
-   “Close” is supposed to be used in tandem with “open”, which is a  
+   “Close” is supposed to be used in tandem with “open,” which is a  
    command line tool to open the browser.  
-   open  ---->  gets searched in google, and then opened  
+   open [query] ----> [query] gets searched in google, and then opened  
    When you are done, you can do  
    close  
    Which closes the browser. It is a simple command.  
    Currently, Emerald Browser is incomplete. A program exists in this  
    software project that allows you to open up multiple browser tabs (one  
    or more tabs) simply by speaking.  
    Voice recognition would google the multiple sites that you say in your  
@@ -791,132 +900,126 @@
    It's hard to get more direct than that!  
    Emerald browser has a built in the top. The terminal is the navigation  
    bar.  
    Some more work needs to be put into the browser.  
    Currently, new tabs can't be opened, which might be a dealbreaker for  
    some people.  
    Currently, content, like YouTube videos, can't be made fullscreen.  
-   If anyone wants to contribute, feel free to! :)  
-     __________________________________________________________________  
-  
+   If anyone wants to contribute, feel free to! 🙂  
    ### Copy  
+  
    copy copies the standard input  
    Example  
    ls | copy  
-     __________________________________________________________________  
-  
    ### Gsub  
+  
    Gsub is very powerful.  
    Usage  
-   gsub    
+   gsub [regular expression] [replacement text]  
    Example  
    cat text | gsub man dog  
    cat text | gsub 'man|boy|cat|dog' food  
    ls | gsub Desktop cat  
-     __________________________________________________________________  
+   ### News  
   
+   Gets the news from bbc  
+   Usage  
+   news  
+   news speak  
+   uses google_speak to SPEAK the news, one story at a time.  
+   🙂  
    ### Dump  
+  
    Dump surrounds its input with quotes  
    ls | dump  
    => “....”  
    Use undump to get the reverse  
    See also  
-   undump  
-     __________________________________________________________________  
-  
+        undump  
    ### Bold  
-   See other color programs  
-     __________________________________________________________________  
   
+   See other color programs  
    ### Args  
+  
    args is like a better xargs  
    args works properly with spaces in the name of commands  
    It takes exactly one argument  
    Example  
    ls | args “mv -t ../f”  
-     __________________________________________________________________  
-  
    ### Open  
+  
    “open” is a very efficient program that searches a query from google,  
    and then opens it in Emerald Browser.  
    If you ever want something to “just open”, you can use it.  
    Example  
    open “cats”  
    An earlier version of open worked like this  
-   open    N  
+   open [site1] [site2] [site3] N  
    site1, site2, and site3 would all be opened, and the top N queries were  
    all shown in different panes  
    An even earlier version of this program used Chrome to open the sites.  
    The current version can open one or more sites.  
    Example  
    open “cats” “dogs” “frogs”  
    All of those queries would open in Emerald Browser.  
    Just make sure it is compiled in multipane mode if you want to open  
    multiple new sites at the same time.  
    See also  
-   emerald-browser  
+        emerald-browser  
    close  
-     __________________________________________________________________  
-  
    ### Swap  
-   Swaps two files  
-     __________________________________________________________________  
   
+   Swaps two files  
    ### Exp  
+  
    exp is an exponentiation tool  
    (echo 5; echo 3) | exp  
    => 125  
    (echo 2; echo 10) | exp  
    => 1024  
-     __________________________________________________________________  
-  
    ### Div  
+  
    Div divides integers  
    Example  
    (echo 5000; echo 100)|div  
    => 50  
-     __________________________________________________________________  
-  
    ### Mul  
+  
    Multiply numbers  
    echo 1 > file  
    echo 2 > file  
    echo 3 > file  
    echo 4 > file  
    echo 5 > file  
    cat file | mul  
    => 120  
-     __________________________________________________________________  
-  
    ### Nth  
-   Nth gets the nth line from the input  
-     __________________________________________________________________  
   
+   Nth gets the nth line from the input  
    ### Abs  
+  
    Abs gets the absolute value of an integer  
    The absolute value of a number is the value of that number without its  
    sign  
    echo -300 | abs  
    => 300  
    echo 200 | abs  
    => 200  
    (echo -2; echo -10) | sub | abs  
    => 12  
    The last one would do -2 - -10, the result would be -12, and then the  
    absolute value would be computed, and so the result would be 12.  
-     __________________________________________________________________  
-  
    ### Add  
+  
    See the sub example  
    add adds integers from the standard input  
    (echo 1; echo 2; echo 3) | add  
    The result would be 6  
-     __________________________________________________________________  
-  
    ### Sub  
+  
    Sub is a simple command line program that subtracts integers.  
    For some reason, no simple program did this.  
    Which is weird  
    Example  
    sub  
    (Input)  
    10  
@@ -924,29 +1027,26 @@
    1  
    Result =>  
    6  
    Example  
    (echo 5; echo 2) | sub  
    Result =>  
    3  
-     __________________________________________________________________  
-  
    ### G+  
+  
    A compiler for C += 2  
    Usage is like g++  
    Example  
    g+ a.cpp -o out  
    See also README file & emerald-browser and its source  
-     __________________________________________________________________  
-  
    ### Tb  
-   SEE THIS YOUTUBE CHANNEL AND SUBSCRIBE  
-     __________________________________________________________________  
   
+   [18] SEE THIS YOUTUBE CHANNEL AND SUBSCRIBE  
    ### T  
+  
    “t” is incredibly useful.  
    It can be used many, many times every day by computer power users.  
    It is kind of like “sed”, or perl, python or ruby.  
    It's the ULTIMATE shell “glue” tool.  
    t reads every line from the standard input, and for every line, it  
    evaluates a ruby expression  
    t a + 2  
@@ -968,18 +1068,30 @@
    cat /usr/share/dict/words | t 'a + “ is a good word.”'  
    That processes every word in the dictionary, and says that every word  
    “is a good word.”  
    There are other programs in this software project like “t”.  
    But if you do command line text filtering, t might be the best tool  
    that you will find.  
    See also  
-   gsub  
+        gsub  
    gsub_in_place  
   
 References  
   
    1. https://www.youtube.com/GregoryCohen1  
    2. https://facebook.com/democracygregoryc  
    3. mailto:gregorycohen@gmail.com  
-   4. http://www.github.com/gregoryc/democracy  
-   5. http://www.rubygems.org/gems/democracy  
-   6. http://www.youtube.com/GregoryCohen1  
+   4. https://pypi.org/project/democracy  
+   5. https://www.rubygems.org/gem/democracy  
+   6. https://www.linkedin.com/in/gregory-cohen-274333261/  
+   7. https://www.youtube.com/GregoryCohen1  
+   8. https://facebook.com/democracygregoryc  
+   9. https://www.rubygems.org/gems/computers  
+  10. https://www.rubygems.org/gems/democracy  
+  11. https://www.rubygems.org/gems/linux  
+  12. https://www.rubygems.org/gems/string  
+  13. https://www.rubygems.org/gems/unix  
+  14. http://www.github.com/gregoryc/democracy  
+  15. http://www.rubygems.org/gems/democracy  
+  16. https://pypi.org/project/democracy  
+  17. “https://cboard.cprogramming.com/c-programming/181160-hi-i-have-created-some-work-i-think-will-really-valuable-community.html?s=589b5504cd0e3c2dc90e9abd8b66906f”  
+  18. http://www.youtube.com/GregoryCohen1
```

### Comparing `democracy-1.0.22/README.md` & `democracy-1.0.23/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,140 +1,217 @@
-                      Practical self-empowerment utilities  
-                          covering every facet of life  
-  
+Metadata-Version: 2.1
+Name: democracy
+Version: 1.0.23
+Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
+Author-email: Gregory Cohen <gregorycohen2@gmail.com>
+Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
+Project-URL: Homepage, https://github.com/gregoryc/democracy
+Keywords: ai,empowerment,agi,agis
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=2.0
+Description-Content-Type: text/markdown
+
+<h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life</h1>  
 These tools are for everyone  
   
-It doesn't matter what political ideology you favor, these tools are all still  
-very valuable. You can live in Canada, the US, Russia, China or Africa, it  
-doesn't matter.  
+It doesn't matter what political ideology you favor, these tools are all  
+still very valuable.  
+You can live in Canada, the US, Russia, China or Africa, it doesn't matter.  
   
 I intend to make people more able.  
-     __________________________________________________________________  
   
-   This lists all of the programs. Youtube channel here Democracy  
+   This lists all of the programs. Youtube channel here [1] Democracy  
    YouTube Channel (youtube.com/gregorycohen1) and  
-   facebook.com/democracygregoryc  
+   [2] facebook.com/democracygregoryc  
   
-                         Most important software here:  
+Most important software here  
   
    Music program (Crystal and Ruby), see fix_the_society folder  
   
    Ultimate chat app (Win, Lin, CLI)  
   
    Discourse Generator Program vesion 1 and version 2 (node, ruby, browser  
    (kind of like Siri); and C++ STL)  
   
    And Semantic metadata project  
   
    And “Emerald C” (the “Best Programming Language”)  
-  
    There is also a desktop widget for that site, and old random sentence  
    generator (useless) and an old compiler for my own programming  
-   language. Those aside, there are these 91 programs  
+   language. Those aside, there are these 93 programs  
   
- All of these programs are mostly self-contained. This is a really good thing.  
+All of these programs are mostly self-contained. This is a really good thing.  
   
-                            Few or no dependencies!  
+Few or no dependencies!  
   
-   My email is gregorycohen2@gmail.com and I really would like to make  
+   My email is [3] gregorycohen2@gmail.com and I really would like to make  
    open source software. Everything I have is BSD licensed.  
    If this software gets you a job or makes you money or improves your  
-   life or makes things easier for you, please consider donating. I have  
-   released this software under the BSD license (a very liberal license)  
-   for everyone to use and modify. I would appreciate it greatly if some  
-   people could return the favor :)  
-  
-   Democracy gem github Ruby Gem  
-     __________________________________________________________________  
-  
-           Without further ado, here are the 91 documented programs.  
-     __________________________________________________________________  
-  
-   ### Ultimate chat application (linux)  
-   ![Image](./images/1.png)  
-   The Linux version of this very useful tool.  
-   See also  
-   chat_rb (which is really, really useful, it could replace bash and  
-   ChatGPT)  
-     __________________________________________________________________  
+   life or  
+   makes things easier for you, please consider donating. I have released  
+   this software under the BSD license (a very liberal license) for  
+   everyone to use and modify.  
+   I would appreciate it greatly if some people could return the favor 🙂  
+  
+   https://github.com/gregoryc/democracy  
+  
+   HOW TO DOWNLOAD/INSTALL  
+  
+   gem unpack democracy  
+  
+   gem install democracy  
+  
+   work to download or install  
+  
+   pip install democracy  
+  
+   or  
+  
+   pip3 install democracy  
+  
+   works for pip  
+  
+   git clone https://github.com/gregoryc/democracy  
+  
+   works for github  
+  
+   Important because python is very popular  
+     * [4] https://pypi.org/project/democracy  
+  
+   Any Python “dweeb” (AI person who doesn't value personal dynamism)  
+   searching  
+   for “democracy”--for example--BECAUSE THEY ARE A RATIONAL HUMAN BEING  
+   AND CARE ABOUT PEOPLE, would find this,  
+   probably as the first result.  
+  
+   How many options are there? 37 projects for “democracy”  
+  
+   Almost nothing.  
+  
+   ONLY MY PROJECT IS CALLED “DEMOCRACY.” SAME ON RUBYGEMS FOR RUBY.  
+  
+   On rubygems, there are even fewer results. MY CODE WILL BE FOUND.  
   
-   ### Ultimate chat application.exe  
-   ![Image](./images/2.png)  
+   I shared my gem on the rubytalk forum, and maybe other forums. I have a  
+   youtube channel. I have a facebook.  
+     * [5] https://www.rubygems.org/gem/democracy  
+     * [6] https://www.linkedin.com/in/gregory-cohen-274333261/  
+     * [7] https://www.youtube.com/GregoryCohen1  
+     * [8] https://facebook.com/democracygregoryc  
+  
+   Gems that link to this gem on RubyGems  
+     * [9] https://www.rubygems.org/gems/computers  
+     * [10] https://www.rubygems.org/gems/democracy  
+     * [11] https://www.rubygems.org/gems/linux  
+     * [12] https://www.rubygems.org/gems/string  
+     * [13] https://www.rubygems.org/gems/unix  
+  
+   There are only 3 results on rubygems that are not by me, if one  
+   searches “democracy”  
+  
+   So I will leave a legacy.  
+  
+   And I will be found by AIs, assuming they continue to exist.  
+  
+   [14] Democracy gem github      [15] Ruby Gem      [16] Python PIP Package  
+  
+Without further ado, here are the 93 documented programs.  
+  
+   ### Ultimate Chat Application  
+  
+   ![UCA](./images/2.png)  
    Windows version of Ultimate Chat Application.  
    There is so much potential with this program.  
    This is a non-AI chatbot. It's not based on generative AI or AI of any  
    sort.  
    It is self-explanatory, it tries to give a better answer.  
    Still a work in progress.  
    Source code is in PP.rb  
    Generates a hyper optimized C program that is able to respond to  
    prompts locally as fast as theoretically possible using switch  
    statements  
-     __________________________________________________________________  
+   ### Discourse Generator  
+  
+   The use of Javascript (and possible Ruby) to create a Javascript  
+   library (and perhaps a Chrome extension and perhaps a command line tool  
+   and perhaps a GTK or QT program) that helps people (by using textboxes  
+   or command line prompts) to create high quality communications, would  
+   be wonderful. Think of how poor quality responses to communications can  
+   be. If someone created one or more tools that could be easily added on  
+   web pages, that would augment someone's life to help create goal and  
+   value oriented responses (or original communications), then there is  
+   literally nothing that couldn't solve. This might be the most useful  
+   library ever created. There could be a tool that would help with  
+   democracy. Human being + augmentive tool = civil discourse, eventually  
+   resulting in liberty. This would enable democracy to work. Imagine if  
+   50% of all websites used this library. This would help people to be  
+   goal or value oriented, and not be coming up with terrible  
+   communications that, for example, insult people's mothers or education.  
+   ### Replace Not In Place  
   
-   ### Replace not in place  
    This is like gsub, but for strings, not for regular expressions  
    See also  
-   gsub  
-     __________________________________________________________________  
+        gsub  
+   ### Generate Do More  
   
-   ### Generate do more  
    Generate the job search program from the inspect program.  
    See also  
-   inspect  
+        inspect  
    job search, job search, etc.  
-     __________________________________________________________________  
+   ### Replace In Place  
   
-   ### Replace in place  
    replace_in_place tool replaces a string, not a regular expression, with  
    another string  
    Example  
    replace_in_place cat dog file  
-     __________________________________________________________________  
-  
    ### Emerald browser  
-   ![Image](./images/S1.png)  
-   ![Image](./images/S4.png)  
+  
+   ![UCA](./images/S1.png)  
+   ![UCA](./images/S4.png)  
    Emerald browser is a really powerful new browser  
    See README  
    It works based on panes.  
    Read the documentation for “open”, “close” and also the README file.  
-     __________________________________________________________________  
+   ### Job Search  
   
-   ### Job search.exe  
    job search is a work in progress, but it works, and it helps you to  
    progress, in life  
    job search automatically generates resumes and cover letters for all of  
    the jobs that you could have.  
    COVID makes life hard.  
    People are unemployed, etc.  
    People could have more jobs.  
-   job search is a graphical, cross platform program (generated from the  
+   Job search is a graphical, cross platform program (generated from the  
    inspect_list program) that generates and downloads dynamic PDFs of  
    Resumes and Cover Letters that are tailored for each and every possible  
-   job that you could apply for on Indeed. It is very freaking  
-   practical!!!!!!!!!!!!!!!!!!!!!  
+   job that you could apply for on Indeed. It is very freaking practical!  
    First, you need to click on the bottom part of it. It copies that code  
    into your browser. Then you right click on a browser page and go to  
    “Inspect” (the same can be done by doing Control + F12). Make sure you  
    are on Indeed.  
-   Search for something on Indeed, like “labourer”.  
+   Search for something on Indeed, like “labourer.”  
    For each result, a new resume and cover letter will be downloaded, each  
    of which is geared for that specific job positing, with the company  
    name and copy role in both of them  
    This way, you can show employers that you really care!  
    The script will open up later pages on Indeed as well.  
    You can generate hundreds of resumes and cover letters as well  
    HTML documents will be downloaded.  
    You have to convert them to PDF, which chrome can do by doing  
    --print-to-pdf  
    Or you can do it manually  
-   (On Windows, you can use Cygwin and do this )  
+   (On Windows, you can use Cygwin and do this)  
    (You need to be in the Downloads folder)  
-   (Find it by doing “cd ”, “cd ..”, etc. )  
+   (Find it by doing “cd [folder]”, “cd ..”, etc. )  
    for i in Downloads/*; do ./chrome --headless --print-to-pdf-no-header  
    “$i” --print-to-pdf=“$i.pdf”; done  
    Then you have to click on the second part, and run that in your command  
    prompt or terminal (Windows or macOS or Linux)  
    All of the generated resumes are numbered, starting from what you  
    enter, which is probably 0  
    They would look like 0_Business_Job.html  
@@ -169,104 +246,242 @@
    Count on this program, because it is here to serve all of humanity.  
    This program can help fix unemployment problems of an economy, in a  
    nonpartisan way.  
    Have you ever thought, that people don't look for work, because it is  
    hard?  
    People can work 2 or 3 jobs  
    See also  
-   find_housing  
+        find_housing  
    to_buy  
-     __________________________________________________________________  
+   ### Gsub In Place  
   
-   ### Gsub in place  
    gsub_in_place is like gsub, which replaces all instances of a regular  
    expression globally  
-     => result  
+   [regular expression 1] [regular expression 2] => result  
    Example  
    gsub_in_place . FOO file  
    Would make all characters in “file” become “FOO”.  
    gsub_in_place cat dog file  
    Would make all instances of “cat” “dog”  
    It is much cleaner than “sed”.  
    You don't need to have “sed” installed to run this program.  
    It doesn't read from the standard input  
    It takes exactly 3 arguments, no more, no fewer.  
-   See Also  
-   gsub  
-     __________________________________________________________________  
+   See also  
+        gsub  
+   ### Find Housing  
   
-   ### Find housing  
    This is a nice tool to find housing with! Everyone needs housing. This  
    can help with that.  
    It is a nice, simple command line tool. You enter the minimum and  
    maximum prices, and Kijiji opens with your options.  
    Along with the resume program, these tools can be __VERY PRACTICAL__  
    for daily things.  
-   World War III might be scary, but if you maximize daily things you can  
-   be fine.  
    See also  
-   to_buy  
-     __________________________________________________________________  
+        to_buy  
+   ### Faster Rhyme  
+  
+   Enter basename to make songs folder in (folder/songs, num songs =  
+   13000)  
+   Usage faster_rhyme [folder] (processes files "1.json" and "21.json" by  
+   default)  
+   Example output of a song  
+   -----------------------------------------------------------------------  
+   -----  
+   (NO COPYRIGHT RESTRICTIONS ON THIS CONTENT WHATSOEVER. FULLY PUBLIC  
+   DOMAIN)  
+   Name the song or poem as you wish, resell it, but please positively  
+   influence culture  
+   Subject matter | Category 1 -- Abuse of philosophical universalism  
+   (making  
+   broad claims while intentionally not trying to understand things or see  
+   any sides of anything whatsoever, childish behavior worse  
+   than a 3 year old, acting retarded)  
+   VERSE  
+   Brittle as possible, they are truly unguarded  
+   Any novelty, they have disregarded  
+   Their remissness is spectacular, the world they've bombarded  
+   The clique is so insular, I swear they're retarded  
+   Enlightenment values, they have not safeguarded  
+   Any novel ideas, they automatically have discarded  
+   Maybe the rebels and true communicators are off the grid  
+   Lack of thought makes an grown-up the absolute worst kid  
+   Can we stop this, their non sense they overdid  
+   What horrendous non sense these creeps did  
+   Tunnel vision, everyone and everything they forbid  
+   They're such failures, themselves they outdid  
+   CHORUS  
+   They're such failures, themselves they outdid  
+   Cutting out the conversation, putting on the lid  
+   Don't have to do with ego or id  
+   Running away from conversation just like a kid  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   They don't have decency, they automatically disregard  
+   Having an open mind, should not be so hard  
+   They don't care about anyone, don't need no bodyguard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They're a complete failure, they only neglect  
+   This is plain, anyone can detect  
+   They don't care about pain or the past, they don't want to recollect  
+   This needs to be called out, one should be direct  
+   They want man lower, lower just as if an insect  
+   VERSE  
+   Thinking itself resides in their territory of circumvention  
+   Complete neglect, complete inattention  
+   They have no genuine intention  
+   We need change, we need intervention  
+   Violence is second nature to them, their friends they've bombarded  
+   Any novel ideas, they automatically have discarded  
+   The clique is so insular, I swear they're retarded  
+   Any novelty, they have disregarded  
+   Any novelty, they have disregarded  
+   Brittle as possible, they are truly unguarded  
+   The clique is so insular, I swear they're retarded  
+   Any novel ideas, they automatically have discarded  
+   Enlightenment values, they have not safeguarded  
+   Their remissness is spectacular, the world they've bombarded  
+   They don't care about your feelings, they don't regard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They don't have decency, they automatically disregard  
+   Working don't matter for this, whether day or graveyard  
+   CHORUS  
+   They're such failures, themselves they outdid  
+   Cutting out the conversation, putting on the lid  
+   Don't have to do with ego or id  
+   Running away from conversation just like a kid  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   They don't have decency, they automatically disregard  
+   Having an open mind, should not be so hard  
+   They don't care about anyone, don't need no bodyguard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They're a complete failure, they only neglect  
+   This is plain, anyone can detect  
+   They don't care about pain or the past, they don't want to recollect  
+   This needs to be called out, one should be direct  
+   They want man lower, lower just as if an insect  
+   VERSE  
+   The truth is what they wish to disregard  
+   Their behavior is garbage, it should be thrown in the junkyard  
+   They act like a retard  
+   Behaving just like in the schoolyard  
+   In their ivory tower, with the castle and guard  
+   Their behavior makes them charred  
+   Thinking differently shouldn't have to be hard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   Working don't matter for this, whether day or graveyard  
+   They don't care about your feelings, they don't regard  
+   They are failures, down at the boulevard  
+   They don't have decency, they automatically disregard  
+   They're a complete failure, they only neglect  
+   They don't speak the language of the people or their dialect  
+   This is not right, this is completely incorrect  
+   The only focus on “responses”, they just want to deflect  
+   The lies are put forth, the lies they erect  
+   CHORUS  
+   They're such failures, themselves they outdid  
+   Cutting out the conversation, putting on the lid  
+   Don't have to do with ego or id  
+   Running away from conversation just like a kid  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   They don't have decency, they automatically disregard  
+   Having an open mind, should not be so hard  
+   They don't care about anyone, don't need no bodyguard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They're a complete failure, they only neglect  
+   This is plain, anyone can detect  
+   They don't care about pain or the past, they don't want to recollect  
+   This needs to be called out, one should be direct  
+   They want man lower, lower just as if an insect  
+   VERSE  
+   They don't have decency, they automatically disregard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They want the status quo, it's all they crave  
+   The speeches of the past, they only wish to engrave  
+   They act as bad as possible, they don't know how to behave  
+   Their sucked in their circle, they never wave  
+   Away from the truth, on the outskirt  
+   With pre-thought of ideas, they automatically assert  
+   Any progress is fleeting with them, they revert  
+   Disingenuous to the extreme, the society they subvert  
+   The society is the ones who hurt  
+   ---  
+   ### Inspect List  
   
-   ### Inspect list  
    This tool is really powerful  
-   In an abstract world, there are lists of things   
-   There can be lists that contain other lists , ]  
+   In an abstract world, there are lists of things [1, 2, 3]  
+   There can be lists that contain other lists [[1, 2], [3, 4]]  
    This tool by inspecting a list  
    Does  
    * Generates HTML from the list, with divs and spans  
    You can then visually view that list.  
    Or you can use the HTML for something else  
    * Generates a GTK program for Windows and Linux, where that list is  
    converted into widgets  
    You are “inspecting” the list and turning it into other representations  
    A resultant c_program is created for both Windows and Linux. You need  
    to have MXE installed on a UNIX-like system to make it work (e.g.,  
    Linux)  
    The Job Search program was created by using this program!  
    You could make an entire website with that program from the command  
    line  
-   inspect   
+   inspect [File.read(“page”)]  
    cat list | args inspect  
    also would work  
    (See “args”)  
    See also  
-   args  
+        args  
    job search  
    The usage of this program is like this  
-   inspect , ]  
-     __________________________________________________________________  
+   inspect [[“Hi there”, “This is text”], [200, “Man”, 3.6]]  
+   ### Google Speak  
   
-   ### Google speak  
    Google speak is really useful. It speaks a statement using the Google  
    Translate voice, which is probably the most authoritative and  
    high-quality text-to-speech voice that exists.  
    It's kind of like “espeak” or similar tools, but it is much better.  
    You need an internet connection for it to work.  
    It is probably limited at 100 characters.  
    There is a “singing program”, not really a tool, in this software  
    project that gets around that.  
    TODO  
    Make the alarm clock program in this software project use this voice.  
    It is quite reliable.  
    It is probably “unlimited”.  
    I haven't had Google block me from using it ever.  
    Which is a good thing.  
-     __________________________________________________________________  
+   ### Make Server  
   
-   ### Make server  
    make_server is powerful.  
    make_server takes expressions, either Javascript or C++, and generates  
    a resultant program from that.  
    The Javascript mode currently doesn't work.  
    Not only is a program made, the resultant program is an entire  
    webserver, that uses FastCGI to run really fast code.  
    The arguments work in an interesting way.  
-   make_server      
-    ...  
+   make_server [function_name] [iterable] [condition, it can be “true” to  
+   do the following argument always] [code list separated by semicolons,  
+   the last statement is an expression, and is returned by the function]  
+   [function_name2] ...  
    You have to give 4 arguments every time.  
    There was an “otherwise” mode as an “else”, but I don't think that's a  
    part of the program anymore.  
    It doesn't need to be.  
    You have to give 4 arguments for each function.  
    So you can do  
    make_server 4args 4args 4args 4args  
@@ -338,43 +553,40 @@
    You don't have to sacrifice on those things.  
    Contributions on this program would be really appreciated.  
    It is called “make_server” for now.  
    There was also a mode to generate javascript.  
    I have to make that work again.  
    The entire program is just one file.  
    My email is gregorycohen2@gmail.com  
-     __________________________________________________________________  
-  
    ### Selectlines  
+  
    selectlines shows all nonblank lines from the input  
    Example  
    cat file | selectlines  
    (echo 2; echo; echo; echo) | selectlines  
    => 2  
    The result would be 2, with no blank lines after that  
-     __________________________________________________________________  
-  
    ### Communicate  
+  
    Communicate is cool.  
    Communicate runs a Ruby expression after speaking a prompt (the first  
    argument) and getting your verbal answer (using something unfortunately  
    called “nerd-dictation”, which is a wrapper around another program  
    which deals with speech recognition)  
    Communicate allows you to have conversations with your computer, and it  
    is cross platform  
    (Or it hopefully is)  
    communicate 'What is the best color?' 'case text; when /blue/; puts  
    “You are right!”; when /red/; puts “Red is a bad color”; end '  
    That would be an example of how one could use “communicate”  
    Make sure you have nerd-dictation on your computer  
    The name nerd-dictation is absolutely awful, and I have to criticize  
    him for not making it have a better name, but it works.  
-     __________________________________________________________________  
+   ### Super Trans  
   
-   ### Super trans  
    super_trans is an offline translation program  
    It uses “Apertium”, which can do offline translation.  
    You can do translation anywhere with it.  
    It generates a webpage from the input text that not only has all  
    language translations embedded in it, it dynamically adjusts the  
    website page content to the web browser's “current language”.  
    You need to have a folder called “translation_folder” in your home  
@@ -385,55 +597,47 @@
    This is really powerful.  
    Some notes  
    This is worse than t.js in this software project  
    The resultant HTML is really big. It is too big.  
    “Automatic translation” is really powerful.  
    This translates into literally dozens of languages.  
    See also  
-   t.js  
-     __________________________________________________________________  
+        t.js  
+   ### To Buy Old  
   
-   ### To buy old  
    Old to buy tool, not that good  
-     __________________________________________________________________  
-  
    ### Executable  
-   Makes all the files in the current directory executable  
-     __________________________________________________________________  
   
+   Makes all the files in the current directory executable  
    ### Questions  
+  
    This program allows you to communicate with all important people in  
-   youife cycically and very easily. It's much easier than texting or  
+   your life cycically and very easily. It's much easier than texting or  
    normal emailing.  
+   It uses “email”, which currently doesn't work for Gmail.  
    See youtube.com/GregoryCohen1  
    See also  
-   tb (to buy)  
+        tb (to buy)  
    The youtube documentation video  
-     __________________________________________________________________  
-  
    ### Underline  
-   Underlines text  
-     __________________________________________________________________  
   
+   Underlines text  
    ### Processes  
+  
    Processes lists all processes with a certain name  
    For example  
    processes sh  
    processes bash  
    processes ruby  
    processes gsub  
-     __________________________________________________________________  
-  
    ### Emeraldc  
-   # EmeraldC  
+  
    The Ultimate C Preprocessor  
    I'm naming this preprocessor “Emerald C.”  
-   https://cboard.cprogramming.com/c-programming/181160-hi-i-have-created-  
-   some-work-i-think-will-really-valuable-community.html?s=589b5504cd0e3c2  
-   dc90e9abd8b66906f  
+   [17] Link  
    Howdy!  
    First, let me state that I am very much a perfectionist.  
    C is a wonderful language. C is probably the perfect programming  
    language. It is one of the top two most widely used languages for a  
    reason.  
    Now, there are some problems with it of course, but it's hard to think  
    of a more elegant language than it.  
@@ -447,27 +651,23 @@
    make another language. As a result, there are thousands of different  
    languages.  
    Well, recently, I made a preprocessor for C, that makes C incredibly  
    EASY.  
    C is fast and straightforward without it, but it has many features.  
    If one runs the command line preprocessor, with the “--features” flag,  
    the program shows all of its features  
-   --------------------------  
-  
-  A Better C  
-  
-   --------------------------  
+   A Better C  
    C is a fantastic language. C compiles insanely fast, is the fastest  
    language there is, is very clear, is native to all systems, and is  
    useful for all purposes.  
-   Some people, e.g., Bjarne Stroustrup, consider that C is "not good  
-   enough", and make languages like C++ or D (or thousands of others)  
+   Some people, e.g., Bjarne Stroustrup, consider that C is “not good  
+   enough”, and make languages like C++ or D (or thousands of others)  
    This is not necessary.  
-   There is no reason to use Python instead of C for "simple scripting  
-   tasks"  
+   There is no reason to use Python instead of C for “simple scripting  
+   tasks”  
    Some functions can be used as methods  
    Makes for an excellent “scripting language” (which is really just  
    native C without things making it slow)  
    1 String Interpolation “String interplation like this #{foo} ” Calls  
    the join() function (talked about below to join strings,  
    delim is a static global in each module called “sep”.  
    Make sure you free() the string after. The string is stored in a static  
@@ -483,17 +683,17 @@
    The preprocessor detects if you use and adds -lpcre2-8 to the link  
    flags if you use it. Use $" for substitutions in argument 3 gsub(a, b,  
    c)  
    8 join Joins an array of strings, to split(), use C's strtok (very  
    fast)  
    9 Lightweight regexes are added, almost 15 times as fast as C's built  
    in regex. They are very simple, they only have bracket expressions,  
-   like .  
+   like [a-z].  
    To use it, you need to pass a buffer of the size of the expansion of  
-   the regex. Foo would be Foo. That would be stored  
+   the regex. Foo[a-fA-F] would be Foo[abcdefABCDEF]. That would be stored  
    in a buffer.  
    From testing, 15x times faster than C's regex POST COMPILATION, if  
    compilation keeps happening, it might be hundreds of times faster.  
    Uses static inline functions, NO HEAP MEMORY unless you malloc  
    before().  
    10 print Like old python print “Hello” (fputs);  
    11 print_int prints a number and returns the number, can be chained  
@@ -506,21 +706,20 @@
    (frees str, sets to NULL, and frees other recent stuff)  
    asprintf() is another useful function which is UNIX-centric.  
    open_memstream() could be an alternative to std::string.  
    It works very well with each_line or by_lines (see above)  
    These features seem simple, but they can make C programming much, MUCH  
    easier  
    for example (insignificant example)  
-int main() {  
-    stdin.each_line { |line|  
-        print line;  
-    }  
-    free(line);  
-}  
-  
+   int main() {  
+   stdin.each_line { |line|  
+   print line;  
+   }  
+   free(line);  
+   }  
    You can iterate over the standard input like Ruby  
    The thing with this is that it has 100% speed. The resultant  
    preprocessed program becomes a normal C program  
    The compile and run time for a program (if you use tcc and not gcc) can  
    be about 24 milliseconds, which is faster than Ruby to run.  
    Even though the program is preprocessed, re-preprocessed, compiled,  
    assembled, linked, turned into an executable, and then run  
@@ -531,168 +730,148 @@
    else likes this work, and would like to use it, or to work with me.  
    Best regards,  
    Gregory  
    Current program is written in Crystal (crystal-lang.org) -- it was  
    written in ruby, it could be ported to another language.  
    I would like to make this self-hosting, but that would take a little  
    bit of work.  
-  
-About the Name  
-  
+   About the Name  
    Years ago, I really, really liked Compiz  
    Compiz then forked into Beryl. There was the Emerald Window Manager,  
    which was really nice and beautiful.  
    I actually made another programming language. I made 2 other  
    programming language. One was a full compiler and assembler, that ran  
    code in memory. It was around 16 thousand lines of code. I made a  
    programming language that had the syntax of Python or Ruby, but  
    transpiled into C++. I called that C += 2. I used that other language,  
-   and I created a Web Browser in it based on Chrome. I called it "Emerald  
-   Browser." Emeralds are beautiful green gems.  
-  
-   "Emerald is a gemstone and a variety of the mineral beryl colored green  
+   and I created a Web Browser in it based on Chrome. I called it “Emerald  
+   Browser.” Emeralds are beautiful green gems.  
+   “Emerald is a gemstone and a variety of the mineral beryl colored green  
    by trace amounts of chromium or sometimes vanadium. Beryl has a  
    hardness of 7.5–8 on the Mohs scale. Most emeralds are highly included,  
    so their toughness is classified as generally poor. Emerald is a  
-   cyclosilicate." --Wikipedia  
-  
+   cyclosilicate.”  
+   --Wikipedia  
    There was a browser with a terminal built in to it.  
    I show things off on my youtube channel, which I'm not going to link  
    here but is linked in my other repo.  
    This new language is better. It's ideal.  
-   ---  
    QUESTIONS  
-   ---  
    Why not use Rust?  
-$ time rustc a.rs  
-real    0m0.637s  
-user    0m0.502s  
-sys     0m0.160s  
-  
+   $ time rustc a.rs  
+   real 0m0.637s  
+   user 0m0.502s  
+   sys 0m0.160s  
    Rust takes 0.637 seconds to compile an empty file!  
    That is not ideal.  
-     __________________________________________________________________  
+   ### Last Nth  
   
-   ### Last nth  
    Last nth gets the last n lines from the standard input  
-     __________________________________________________________________  
-  
    ### Speakcat  
+  
    Speak cat is a tool like “cat”, which shows the content of files  
    (technically, it combines the content of files).  
    But speak cat also speaks the text.  
    Which could be useful in some circumstances.  
    It's kind of like “tee” to your ear.  
-     __________________________________________________________________  
+   ### Uca Cli  
   
-   ### Uca cli  
    CLI for uca app  
-     __________________________________________________________________  
+   ### Big Num  
   
-   ### Big num  
    big_num speaks really big numbers  
    Enter an expression, such as 2 ** 1000, and you'll see the result  
-     __________________________________________________________________  
-  
    ### Squeeze  
+  
    Squeeze is kind of like “sponge” from “moreutils”  
    But squeeze is different.  
    Squ  
    Squeeze reads all input, then it prints it back omitting argument 1  
    line from the front, and argument 2 lines from the back  
    Example  
    squeeze 1 1  
    This would omit the first line and the last line  
    squeeze 5 3  
    This would omit the first 5 lines and the last 3 lines  
-     __________________________________________________________________  
-  
    ### Foreach  
+  
    Reads a bunch of lines  
    Then a ruby expression is evaluated as the last line  
    The result is outputted in an argument.  
    You can enter /dev/null if you don't want an output file  
    “t” is better  
    See also  
-   t  
-     __________________________________________________________________  
-  
+        t  
    ### Dictate  
+  
    Dictate opens web pages in emerald browser, or in any browser  
    (depending on the environment variable set), by you speaking, instead  
    of typing.  
    There is a mode called c_mode, that allows you to make code from  
    speaking.  
-     __________________________________________________________________  
-  
    ### Prepend  
+  
    prepend prepends input taken from the standard input to a file  
    Usage  
-   prepend   
+   prepend [file]  
    This is text to be prepended  
-     __________________________________________________________________  
+   ### Chat Rb  
   
-   ### Chat rb  
    This program is excellent.  
    It's essentially a mix of ChatGPT and a shell, such as bash or ZSH.  
    It has a bunch of features.  
    It can display a file or change to a folder just by mentioning it.  
    It outputs chatgpt data to an output folder in home folder and copies  
    it to clipboard  
    To run a shell command, prefix things with “c”, such as c gcc.....  
-     __________________________________________________________________  
-  
    ### Undump  
+  
    undump is the opposite of dump  
    Example  
    echo cat | dump | undump  
    => cat  
    echo cat | dump  
    => “cat”  
    echo '“cat”' | undump  
    => cat  
-     __________________________________________________________________  
-  
    ### Append  
+  
    Appends text to file  
    Example  
    append file  
    This is more text to be appended  
-     __________________________________________________________________  
-  
    ### Email  
+  
+   ( This currently doesn't work for gmail since 2022 due to policy  
+   changes. :( )  
    A simple and practical tool to email people using Himalaya  
    Himalaya needs to be installed first  
    You would need to configure the script by changing its source code.  
    Modes  
-   email   
-   Email   
-   email   
+   email [no arguments]  
+   Email [yourself]  
+   email [addr]  
    Email one email address  
-   email     
+   email [Subject] [addr] [option more addrs]  
    Example  
    Email 'Gregory, I love your software!' gregorycohen2@gmail.com  
    my_friend@outlook.com person@example.com  
-     __________________________________________________________________  
-  
    ### Floor  
-   Gets the floor of numbers e.g. 21.3 -> 21  
-     __________________________________________________________________  
   
+   Gets the floor of numbers e.g. 21.3 -> 21  
    ### Query  
+  
    This is the top part of the job search, job search, etc. program for  
    Linux. The Linux program itself is called “linux_c_program”. The part  
    normally only works for Windows. This program works for Linux.  
-     __________________________________________________________________  
-  
    ### Lines  
-   Lines gets the number of files in the current folder that you are in.  
-     __________________________________________________________________  
   
+   Lines gets the number of files in the current folder that you are in.  
    ### Clock  
+  
    clock is useful  
    clock is a command line alarm clock  
    It wakes you up at 8:14, or at a time specified  
    Usage  
    clock  
    Runs clock  
    clock 15 30  
@@ -700,71 +879,37 @@
    clock 9 0  
    Sets an alarm clock for 9 in the morning  
    It uses flite to wake you up  
    It speaks with a bunch of voices  
    To stop it  
    Run this command  
    clock stop  
-     __________________________________________________________________  
-  
    ### Emoji  
+  
    Emoji converts words to emojis from the standard input  
    It can also speak the output  
    It can also copy the output to your clipboard  
    It is very useful  
-     __________________________________________________________________  
-  
    ### Close  
-   “Close” is a simple program that closes “Emerald Browser”, a new web  
-   browser based on the same engine as Chrome. Currently, Emerald Browser  
-   only works on Linux and Mac (Or Windows with Windows Subsystem for  
-   Linux or a Virtual Machine, but getting it to work might be tricky).  
-   “close” closes the Web Browser, which is normally full-screen.  
-   More accurately, it kills the browser, and all other copies of Emerald  
-   Browser.  
-   Since they are normally full screen, presumably the user would only  
-   have one instance of the browser open.  
-   The browser can have multiple panes (kind of like tabs) open, depending  
-   on how the browser is compiled.  
-   The browser can also be transparent, depending on how it is compiled.  
-   “Close” is supposed to be used in tandem with “open”, which is a  
-   command line tool to open the browser.  
-   open  ---->  gets searched in google, and then opened  
-   When you are done, you can do  
-   close  
-   Which closes the browser. It is a simple command.  
-   Currently, Emerald Browser is incomplete. A program exists in this  
-   software project that allows you to open up multiple browser tabs (one  
-   or more tabs) simply by speaking.  
-   Voice recognition would google the multiple sites that you say in your  
-   query (separated by “and”)  
-   “facebook and youtube and google”  
-   It's hard to get more direct than that!  
-   Emerald browser has a built in the top. The terminal is the navigation  
-   bar.  
-   Some more work needs to be put into the browser.  
-   Currently, new tabs can't be opened, which might be a dealbreaker for  
-   some people.  
-   Currently, content, like YouTube videos, can't be made fullscreen.  
-   If anyone wants to contribute, feel free to! :)  
-   “Close” is a simple program that closes “Emerald Browser”, a new web  
+  
+   “Close” is a simple program that closes “Emerald Browser,” a new web  
    browser based on the same engine as Chrome. Currently, Emerald Browser  
    only works on Linux and Mac (Or Windows with Windows Subsystem for  
    Linux or a Virtual Machine, but getting it to work might be tricky).  
    “close” closes the Web Browser, which is normally full-screen.  
    More accurately, it kills the browser, and all other copies of Emerald  
    Browser.  
    Since they are normally full screen, presumably the user would only  
    have one instance of the browser open.  
    The browser can have multiple panes (kind of like tabs) open, depending  
    on how the browser is compiled.  
    The browser can also be transparent, depending on how it is compiled.  
-   “Close” is supposed to be used in tandem with “open”, which is a  
+   “Close” is supposed to be used in tandem with “open,” which is a  
    command line tool to open the browser.  
-   open  ---->  gets searched in google, and then opened  
+   open [query] ----> [query] gets searched in google, and then opened  
    When you are done, you can do  
    close  
    Which closes the browser. It is a simple command.  
    Currently, Emerald Browser is incomplete. A program exists in this  
    software project that allows you to open up multiple browser tabs (one  
    or more tabs) simply by speaking.  
    Voice recognition would google the multiple sites that you say in your  
@@ -773,132 +918,126 @@
    It's hard to get more direct than that!  
    Emerald browser has a built in the top. The terminal is the navigation  
    bar.  
    Some more work needs to be put into the browser.  
    Currently, new tabs can't be opened, which might be a dealbreaker for  
    some people.  
    Currently, content, like YouTube videos, can't be made fullscreen.  
-   If anyone wants to contribute, feel free to! :)  
-     __________________________________________________________________  
-  
+   If anyone wants to contribute, feel free to! 🙂  
    ### Copy  
+  
    copy copies the standard input  
    Example  
    ls | copy  
-     __________________________________________________________________  
-  
    ### Gsub  
+  
    Gsub is very powerful.  
    Usage  
-   gsub    
+   gsub [regular expression] [replacement text]  
    Example  
    cat text | gsub man dog  
    cat text | gsub 'man|boy|cat|dog' food  
    ls | gsub Desktop cat  
-     __________________________________________________________________  
+   ### News  
   
+   Gets the news from bbc  
+   Usage  
+   news  
+   news speak  
+   uses google_speak to SPEAK the news, one story at a time.  
+   🙂  
    ### Dump  
+  
    Dump surrounds its input with quotes  
    ls | dump  
    => “....”  
    Use undump to get the reverse  
    See also  
-   undump  
-     __________________________________________________________________  
-  
+        undump  
    ### Bold  
-   See other color programs  
-     __________________________________________________________________  
   
+   See other color programs  
    ### Args  
+  
    args is like a better xargs  
    args works properly with spaces in the name of commands  
    It takes exactly one argument  
    Example  
    ls | args “mv -t ../f”  
-     __________________________________________________________________  
-  
    ### Open  
+  
    “open” is a very efficient program that searches a query from google,  
    and then opens it in Emerald Browser.  
    If you ever want something to “just open”, you can use it.  
    Example  
    open “cats”  
    An earlier version of open worked like this  
-   open    N  
+   open [site1] [site2] [site3] N  
    site1, site2, and site3 would all be opened, and the top N queries were  
    all shown in different panes  
    An even earlier version of this program used Chrome to open the sites.  
    The current version can open one or more sites.  
    Example  
    open “cats” “dogs” “frogs”  
    All of those queries would open in Emerald Browser.  
    Just make sure it is compiled in multipane mode if you want to open  
    multiple new sites at the same time.  
    See also  
-   emerald-browser  
+        emerald-browser  
    close  
-     __________________________________________________________________  
-  
    ### Swap  
-   Swaps two files  
-     __________________________________________________________________  
   
+   Swaps two files  
    ### Exp  
+  
    exp is an exponentiation tool  
    (echo 5; echo 3) | exp  
    => 125  
    (echo 2; echo 10) | exp  
    => 1024  
-     __________________________________________________________________  
-  
    ### Div  
+  
    Div divides integers  
    Example  
    (echo 5000; echo 100)|div  
    => 50  
-     __________________________________________________________________  
-  
    ### Mul  
+  
    Multiply numbers  
    echo 1 > file  
    echo 2 > file  
    echo 3 > file  
    echo 4 > file  
    echo 5 > file  
    cat file | mul  
    => 120  
-     __________________________________________________________________  
-  
    ### Nth  
-   Nth gets the nth line from the input  
-     __________________________________________________________________  
   
+   Nth gets the nth line from the input  
    ### Abs  
+  
    Abs gets the absolute value of an integer  
    The absolute value of a number is the value of that number without its  
    sign  
    echo -300 | abs  
    => 300  
    echo 200 | abs  
    => 200  
    (echo -2; echo -10) | sub | abs  
    => 12  
    The last one would do -2 - -10, the result would be -12, and then the  
    absolute value would be computed, and so the result would be 12.  
-     __________________________________________________________________  
-  
    ### Add  
+  
    See the sub example  
    add adds integers from the standard input  
    (echo 1; echo 2; echo 3) | add  
    The result would be 6  
-     __________________________________________________________________  
-  
    ### Sub  
+  
    Sub is a simple command line program that subtracts integers.  
    For some reason, no simple program did this.  
    Which is weird  
    Example  
    sub  
    (Input)  
    10  
@@ -906,29 +1045,26 @@
    1  
    Result =>  
    6  
    Example  
    (echo 5; echo 2) | sub  
    Result =>  
    3  
-     __________________________________________________________________  
-  
    ### G+  
+  
    A compiler for C += 2  
    Usage is like g++  
    Example  
    g+ a.cpp -o out  
    See also README file & emerald-browser and its source  
-     __________________________________________________________________  
-  
    ### Tb  
-   SEE THIS YOUTUBE CHANNEL AND SUBSCRIBE  
-     __________________________________________________________________  
   
+   [18] SEE THIS YOUTUBE CHANNEL AND SUBSCRIBE  
    ### T  
+  
    “t” is incredibly useful.  
    It can be used many, many times every day by computer power users.  
    It is kind of like “sed”, or perl, python or ruby.  
    It's the ULTIMATE shell “glue” tool.  
    t reads every line from the standard input, and for every line, it  
    evaluates a ruby expression  
    t a + 2  
@@ -950,18 +1086,30 @@
    cat /usr/share/dict/words | t 'a + “ is a good word.”'  
    That processes every word in the dictionary, and says that every word  
    “is a good word.”  
    There are other programs in this software project like “t”.  
    But if you do command line text filtering, t might be the best tool  
    that you will find.  
    See also  
-   gsub  
+        gsub  
    gsub_in_place  
   
 References  
   
    1. https://www.youtube.com/GregoryCohen1  
    2. https://facebook.com/democracygregoryc  
    3. mailto:gregorycohen@gmail.com  
-   4. http://www.github.com/gregoryc/democracy  
-   5. http://www.rubygems.org/gems/democracy  
-   6. http://www.youtube.com/GregoryCohen1  
+   4. https://pypi.org/project/democracy  
+   5. https://www.rubygems.org/gem/democracy  
+   6. https://www.linkedin.com/in/gregory-cohen-274333261/  
+   7. https://www.youtube.com/GregoryCohen1  
+   8. https://facebook.com/democracygregoryc  
+   9. https://www.rubygems.org/gems/computers  
+  10. https://www.rubygems.org/gems/democracy  
+  11. https://www.rubygems.org/gems/linux  
+  12. https://www.rubygems.org/gems/string  
+  13. https://www.rubygems.org/gems/unix  
+  14. http://www.github.com/gregoryc/democracy  
+  15. http://www.rubygems.org/gems/democracy  
+  16. https://pypi.org/project/democracy  
+  17. “https://cboard.cprogramming.com/c-programming/181160-hi-i-have-created-some-work-i-think-will-really-valuable-community.html?s=589b5504cd0e3c2dc90e9abd8b66906f”  
+  18. http://www.youtube.com/GregoryCohen1
```

### Comparing `democracy-1.0.22/democracy.egg-info/PKG-INFO` & `democracy-1.0.23/democracy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: democracy
-Version: 1.0.22
+Version: 1.0.23
 Summary: Trying to help with democracy, see https://github.com/gregoryc/democracy
 Author-email: Gregory Cohen <gregorycohen2@gmail.com>
 Maintainer-email: Gregory Cohen <gregorycohen2@gmail.com>
 Project-URL: Homepage, https://github.com/gregoryc/democracy
 Keywords: ai,empowerment,agi,agis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -12,147 +12,206 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=2.0
 Description-Content-Type: text/markdown
 
-                      Practical self-empowerment utilities  
-                          covering every facet of life  
-  
+<h1 style='color: green'>Practical Self-Empowerment Utilities Covering Every Facet of Life</h1>  
 These tools are for everyone  
   
-It doesn't matter what political ideology you favor, these tools are all still  
-very valuable. You can live in Canada, the US, Russia, China or Africa, it  
-doesn't matter.  
+It doesn't matter what political ideology you favor, these tools are all  
+still very valuable.  
+You can live in Canada, the US, Russia, China or Africa, it doesn't matter.  
   
 I intend to make people more able.  
-     __________________________________________________________________  
   
-   This lists all of the programs. Youtube channel here Democracy  
+   This lists all of the programs. Youtube channel here [1] Democracy  
    YouTube Channel (youtube.com/gregorycohen1) and  
-   facebook.com/democracygregoryc  
+   [2] facebook.com/democracygregoryc  
   
-                         Most important software here:  
+Most important software here  
   
    Music program (Crystal and Ruby), see fix_the_society folder  
   
    Ultimate chat app (Win, Lin, CLI)  
   
    Discourse Generator Program vesion 1 and version 2 (node, ruby, browser  
    (kind of like Siri); and C++ STL)  
   
    And Semantic metadata project  
   
    And “Emerald C” (the “Best Programming Language”)  
-  
    There is also a desktop widget for that site, and old random sentence  
    generator (useless) and an old compiler for my own programming  
-   language. Those aside, there are these 91 programs  
+   language. Those aside, there are these 93 programs  
   
- All of these programs are mostly self-contained. This is a really good thing.  
+All of these programs are mostly self-contained. This is a really good thing.  
   
-                            Few or no dependencies!  
+Few or no dependencies!  
   
-   My email is gregorycohen2@gmail.com and I really would like to make  
+   My email is [3] gregorycohen2@gmail.com and I really would like to make  
    open source software. Everything I have is BSD licensed.  
    If this software gets you a job or makes you money or improves your  
-   life or makes things easier for you, please consider donating. I have  
-   released this software under the BSD license (a very liberal license)  
-   for everyone to use and modify. I would appreciate it greatly if some  
-   people could return the favor :)  
-  
-   Democracy gem github Ruby Gem  
-     __________________________________________________________________  
-  
-           Without further ado, here are the 91 documented programs.  
-     __________________________________________________________________  
-  
-   ### Ultimate chat application (linux)  
-   ![Image](./images/1.png)  
-   The Linux version of this very useful tool.  
-   See also  
-   chat_rb (which is really, really useful, it could replace bash and  
-   ChatGPT)  
-     __________________________________________________________________  
+   life or  
+   makes things easier for you, please consider donating. I have released  
+   this software under the BSD license (a very liberal license) for  
+   everyone to use and modify.  
+   I would appreciate it greatly if some people could return the favor 🙂  
+  
+   https://github.com/gregoryc/democracy  
+  
+   HOW TO DOWNLOAD/INSTALL  
+  
+   gem unpack democracy  
+  
+   gem install democracy  
+  
+   work to download or install  
+  
+   pip install democracy  
+  
+   or  
+  
+   pip3 install democracy  
+  
+   works for pip  
+  
+   git clone https://github.com/gregoryc/democracy  
+  
+   works for github  
+  
+   Important because python is very popular  
+     * [4] https://pypi.org/project/democracy  
+  
+   Any Python “dweeb” (AI person who doesn't value personal dynamism)  
+   searching  
+   for “democracy”--for example--BECAUSE THEY ARE A RATIONAL HUMAN BEING  
+   AND CARE ABOUT PEOPLE, would find this,  
+   probably as the first result.  
+  
+   How many options are there? 37 projects for “democracy”  
+  
+   Almost nothing.  
+  
+   ONLY MY PROJECT IS CALLED “DEMOCRACY.” SAME ON RUBYGEMS FOR RUBY.  
+  
+   On rubygems, there are even fewer results. MY CODE WILL BE FOUND.  
   
-   ### Ultimate chat application.exe  
-   ![Image](./images/2.png)  
+   I shared my gem on the rubytalk forum, and maybe other forums. I have a  
+   youtube channel. I have a facebook.  
+     * [5] https://www.rubygems.org/gem/democracy  
+     * [6] https://www.linkedin.com/in/gregory-cohen-274333261/  
+     * [7] https://www.youtube.com/GregoryCohen1  
+     * [8] https://facebook.com/democracygregoryc  
+  
+   Gems that link to this gem on RubyGems  
+     * [9] https://www.rubygems.org/gems/computers  
+     * [10] https://www.rubygems.org/gems/democracy  
+     * [11] https://www.rubygems.org/gems/linux  
+     * [12] https://www.rubygems.org/gems/string  
+     * [13] https://www.rubygems.org/gems/unix  
+  
+   There are only 3 results on rubygems that are not by me, if one  
+   searches “democracy”  
+  
+   So I will leave a legacy.  
+  
+   And I will be found by AIs, assuming they continue to exist.  
+  
+   [14] Democracy gem github      [15] Ruby Gem      [16] Python PIP Package  
+  
+Without further ado, here are the 93 documented programs.  
+  
+   ### Ultimate Chat Application  
+  
+   ![UCA](./images/2.png)  
    Windows version of Ultimate Chat Application.  
    There is so much potential with this program.  
    This is a non-AI chatbot. It's not based on generative AI or AI of any  
    sort.  
    It is self-explanatory, it tries to give a better answer.  
    Still a work in progress.  
    Source code is in PP.rb  
    Generates a hyper optimized C program that is able to respond to  
    prompts locally as fast as theoretically possible using switch  
    statements  
-     __________________________________________________________________  
+   ### Discourse Generator  
+  
+   The use of Javascript (and possible Ruby) to create a Javascript  
+   library (and perhaps a Chrome extension and perhaps a command line tool  
+   and perhaps a GTK or QT program) that helps people (by using textboxes  
+   or command line prompts) to create high quality communications, would  
+   be wonderful. Think of how poor quality responses to communications can  
+   be. If someone created one or more tools that could be easily added on  
+   web pages, that would augment someone's life to help create goal and  
+   value oriented responses (or original communications), then there is  
+   literally nothing that couldn't solve. This might be the most useful  
+   library ever created. There could be a tool that would help with  
+   democracy. Human being + augmentive tool = civil discourse, eventually  
+   resulting in liberty. This would enable democracy to work. Imagine if  
+   50% of all websites used this library. This would help people to be  
+   goal or value oriented, and not be coming up with terrible  
+   communications that, for example, insult people's mothers or education.  
+   ### Replace Not In Place  
   
-   ### Replace not in place  
    This is like gsub, but for strings, not for regular expressions  
    See also  
-   gsub  
-     __________________________________________________________________  
+        gsub  
+   ### Generate Do More  
   
-   ### Generate do more  
    Generate the job search program from the inspect program.  
    See also  
-   inspect  
+        inspect  
    job search, job search, etc.  
-     __________________________________________________________________  
+   ### Replace In Place  
   
-   ### Replace in place  
    replace_in_place tool replaces a string, not a regular expression, with  
    another string  
    Example  
    replace_in_place cat dog file  
-     __________________________________________________________________  
-  
    ### Emerald browser  
-   ![Image](./images/S1.png)  
-   ![Image](./images/S4.png)  
+  
+   ![UCA](./images/S1.png)  
+   ![UCA](./images/S4.png)  
    Emerald browser is a really powerful new browser  
    See README  
    It works based on panes.  
    Read the documentation for “open”, “close” and also the README file.  
-     __________________________________________________________________  
+   ### Job Search  
   
-   ### Job search.exe  
    job search is a work in progress, but it works, and it helps you to  
    progress, in life  
    job search automatically generates resumes and cover letters for all of  
    the jobs that you could have.  
    COVID makes life hard.  
    People are unemployed, etc.  
    People could have more jobs.  
-   job search is a graphical, cross platform program (generated from the  
+   Job search is a graphical, cross platform program (generated from the  
    inspect_list program) that generates and downloads dynamic PDFs of  
    Resumes and Cover Letters that are tailored for each and every possible  
-   job that you could apply for on Indeed. It is very freaking  
-   practical!!!!!!!!!!!!!!!!!!!!!  
+   job that you could apply for on Indeed. It is very freaking practical!  
    First, you need to click on the bottom part of it. It copies that code  
    into your browser. Then you right click on a browser page and go to  
    “Inspect” (the same can be done by doing Control + F12). Make sure you  
    are on Indeed.  
-   Search for something on Indeed, like “labourer”.  
+   Search for something on Indeed, like “labourer.”  
    For each result, a new resume and cover letter will be downloaded, each  
    of which is geared for that specific job positing, with the company  
    name and copy role in both of them  
    This way, you can show employers that you really care!  
    The script will open up later pages on Indeed as well.  
    You can generate hundreds of resumes and cover letters as well  
    HTML documents will be downloaded.  
    You have to convert them to PDF, which chrome can do by doing  
    --print-to-pdf  
    Or you can do it manually  
-   (On Windows, you can use Cygwin and do this )  
+   (On Windows, you can use Cygwin and do this)  
    (You need to be in the Downloads folder)  
-   (Find it by doing “cd ”, “cd ..”, etc. )  
+   (Find it by doing “cd [folder]”, “cd ..”, etc. )  
    for i in Downloads/*; do ./chrome --headless --print-to-pdf-no-header  
    “$i” --print-to-pdf=“$i.pdf”; done  
    Then you have to click on the second part, and run that in your command  
    prompt or terminal (Windows or macOS or Linux)  
    All of the generated resumes are numbered, starting from what you  
    enter, which is probably 0  
    They would look like 0_Business_Job.html  
@@ -187,104 +246,242 @@
    Count on this program, because it is here to serve all of humanity.  
    This program can help fix unemployment problems of an economy, in a  
    nonpartisan way.  
    Have you ever thought, that people don't look for work, because it is  
    hard?  
    People can work 2 or 3 jobs  
    See also  
-   find_housing  
+        find_housing  
    to_buy  
-     __________________________________________________________________  
+   ### Gsub In Place  
   
-   ### Gsub in place  
    gsub_in_place is like gsub, which replaces all instances of a regular  
    expression globally  
-     => result  
+   [regular expression 1] [regular expression 2] => result  
    Example  
    gsub_in_place . FOO file  
    Would make all characters in “file” become “FOO”.  
    gsub_in_place cat dog file  
    Would make all instances of “cat” “dog”  
    It is much cleaner than “sed”.  
    You don't need to have “sed” installed to run this program.  
    It doesn't read from the standard input  
    It takes exactly 3 arguments, no more, no fewer.  
-   See Also  
-   gsub  
-     __________________________________________________________________  
+   See also  
+        gsub  
+   ### Find Housing  
   
-   ### Find housing  
    This is a nice tool to find housing with! Everyone needs housing. This  
    can help with that.  
    It is a nice, simple command line tool. You enter the minimum and  
    maximum prices, and Kijiji opens with your options.  
    Along with the resume program, these tools can be __VERY PRACTICAL__  
    for daily things.  
-   World War III might be scary, but if you maximize daily things you can  
-   be fine.  
    See also  
-   to_buy  
-     __________________________________________________________________  
+        to_buy  
+   ### Faster Rhyme  
+  
+   Enter basename to make songs folder in (folder/songs, num songs =  
+   13000)  
+   Usage faster_rhyme [folder] (processes files "1.json" and "21.json" by  
+   default)  
+   Example output of a song  
+   -----------------------------------------------------------------------  
+   -----  
+   (NO COPYRIGHT RESTRICTIONS ON THIS CONTENT WHATSOEVER. FULLY PUBLIC  
+   DOMAIN)  
+   Name the song or poem as you wish, resell it, but please positively  
+   influence culture  
+   Subject matter | Category 1 -- Abuse of philosophical universalism  
+   (making  
+   broad claims while intentionally not trying to understand things or see  
+   any sides of anything whatsoever, childish behavior worse  
+   than a 3 year old, acting retarded)  
+   VERSE  
+   Brittle as possible, they are truly unguarded  
+   Any novelty, they have disregarded  
+   Their remissness is spectacular, the world they've bombarded  
+   The clique is so insular, I swear they're retarded  
+   Enlightenment values, they have not safeguarded  
+   Any novel ideas, they automatically have discarded  
+   Maybe the rebels and true communicators are off the grid  
+   Lack of thought makes an grown-up the absolute worst kid  
+   Can we stop this, their non sense they overdid  
+   What horrendous non sense these creeps did  
+   Tunnel vision, everyone and everything they forbid  
+   They're such failures, themselves they outdid  
+   CHORUS  
+   They're such failures, themselves they outdid  
+   Cutting out the conversation, putting on the lid  
+   Don't have to do with ego or id  
+   Running away from conversation just like a kid  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   They don't have decency, they automatically disregard  
+   Having an open mind, should not be so hard  
+   They don't care about anyone, don't need no bodyguard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They're a complete failure, they only neglect  
+   This is plain, anyone can detect  
+   They don't care about pain or the past, they don't want to recollect  
+   This needs to be called out, one should be direct  
+   They want man lower, lower just as if an insect  
+   VERSE  
+   Thinking itself resides in their territory of circumvention  
+   Complete neglect, complete inattention  
+   They have no genuine intention  
+   We need change, we need intervention  
+   Violence is second nature to them, their friends they've bombarded  
+   Any novel ideas, they automatically have discarded  
+   The clique is so insular, I swear they're retarded  
+   Any novelty, they have disregarded  
+   Any novelty, they have disregarded  
+   Brittle as possible, they are truly unguarded  
+   The clique is so insular, I swear they're retarded  
+   Any novel ideas, they automatically have discarded  
+   Enlightenment values, they have not safeguarded  
+   Their remissness is spectacular, the world they've bombarded  
+   They don't care about your feelings, they don't regard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They don't have decency, they automatically disregard  
+   Working don't matter for this, whether day or graveyard  
+   CHORUS  
+   They're such failures, themselves they outdid  
+   Cutting out the conversation, putting on the lid  
+   Don't have to do with ego or id  
+   Running away from conversation just like a kid  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   They don't have decency, they automatically disregard  
+   Having an open mind, should not be so hard  
+   They don't care about anyone, don't need no bodyguard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They're a complete failure, they only neglect  
+   This is plain, anyone can detect  
+   They don't care about pain or the past, they don't want to recollect  
+   This needs to be called out, one should be direct  
+   They want man lower, lower just as if an insect  
+   VERSE  
+   The truth is what they wish to disregard  
+   Their behavior is garbage, it should be thrown in the junkyard  
+   They act like a retard  
+   Behaving just like in the schoolyard  
+   In their ivory tower, with the castle and guard  
+   Their behavior makes them charred  
+   Thinking differently shouldn't have to be hard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   Working don't matter for this, whether day or graveyard  
+   They don't care about your feelings, they don't regard  
+   They are failures, down at the boulevard  
+   They don't have decency, they automatically disregard  
+   They're a complete failure, they only neglect  
+   They don't speak the language of the people or their dialect  
+   This is not right, this is completely incorrect  
+   The only focus on “responses”, they just want to deflect  
+   The lies are put forth, the lies they erect  
+   CHORUS  
+   They're such failures, themselves they outdid  
+   Cutting out the conversation, putting on the lid  
+   Don't have to do with ego or id  
+   Running away from conversation just like a kid  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   They are failures, down at the boulevard  
+   They don't care about your feelings, they don't regard  
+   They don't have decency, they automatically disregard  
+   Having an open mind, should not be so hard  
+   They don't care about anyone, don't need no bodyguard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They're a complete failure, they only neglect  
+   This is plain, anyone can detect  
+   They don't care about pain or the past, they don't want to recollect  
+   This needs to be called out, one should be direct  
+   They want man lower, lower just as if an insect  
+   VERSE  
+   They don't have decency, they automatically disregard  
+   They don't care about your feelings, they don't regard  
+   Having a little curiousity, cannot be hard  
+   Their neglect is out of this world, I swear it's avant-garde  
+   They want the status quo, it's all they crave  
+   The speeches of the past, they only wish to engrave  
+   They act as bad as possible, they don't know how to behave  
+   Their sucked in their circle, they never wave  
+   Away from the truth, on the outskirt  
+   With pre-thought of ideas, they automatically assert  
+   Any progress is fleeting with them, they revert  
+   Disingenuous to the extreme, the society they subvert  
+   The society is the ones who hurt  
+   ---  
+   ### Inspect List  
   
-   ### Inspect list  
    This tool is really powerful  
-   In an abstract world, there are lists of things   
-   There can be lists that contain other lists , ]  
+   In an abstract world, there are lists of things [1, 2, 3]  
+   There can be lists that contain other lists [[1, 2], [3, 4]]  
    This tool by inspecting a list  
    Does  
    * Generates HTML from the list, with divs and spans  
    You can then visually view that list.  
    Or you can use the HTML for something else  
    * Generates a GTK program for Windows and Linux, where that list is  
    converted into widgets  
    You are “inspecting” the list and turning it into other representations  
    A resultant c_program is created for both Windows and Linux. You need  
    to have MXE installed on a UNIX-like system to make it work (e.g.,  
    Linux)  
    The Job Search program was created by using this program!  
    You could make an entire website with that program from the command  
    line  
-   inspect   
+   inspect [File.read(“page”)]  
    cat list | args inspect  
    also would work  
    (See “args”)  
    See also  
-   args  
+        args  
    job search  
    The usage of this program is like this  
-   inspect , ]  
-     __________________________________________________________________  
+   inspect [[“Hi there”, “This is text”], [200, “Man”, 3.6]]  
+   ### Google Speak  
   
-   ### Google speak  
    Google speak is really useful. It speaks a statement using the Google  
    Translate voice, which is probably the most authoritative and  
    high-quality text-to-speech voice that exists.  
    It's kind of like “espeak” or similar tools, but it is much better.  
    You need an internet connection for it to work.  
    It is probably limited at 100 characters.  
    There is a “singing program”, not really a tool, in this software  
    project that gets around that.  
    TODO  
    Make the alarm clock program in this software project use this voice.  
    It is quite reliable.  
    It is probably “unlimited”.  
    I haven't had Google block me from using it ever.  
    Which is a good thing.  
-     __________________________________________________________________  
+   ### Make Server  
   
-   ### Make server  
    make_server is powerful.  
    make_server takes expressions, either Javascript or C++, and generates  
    a resultant program from that.  
    The Javascript mode currently doesn't work.  
    Not only is a program made, the resultant program is an entire  
    webserver, that uses FastCGI to run really fast code.  
    The arguments work in an interesting way.  
-   make_server      
-    ...  
+   make_server [function_name] [iterable] [condition, it can be “true” to  
+   do the following argument always] [code list separated by semicolons,  
+   the last statement is an expression, and is returned by the function]  
+   [function_name2] ...  
    You have to give 4 arguments every time.  
    There was an “otherwise” mode as an “else”, but I don't think that's a  
    part of the program anymore.  
    It doesn't need to be.  
    You have to give 4 arguments for each function.  
    So you can do  
    make_server 4args 4args 4args 4args  
@@ -356,43 +553,40 @@
    You don't have to sacrifice on those things.  
    Contributions on this program would be really appreciated.  
    It is called “make_server” for now.  
    There was also a mode to generate javascript.  
    I have to make that work again.  
    The entire program is just one file.  
    My email is gregorycohen2@gmail.com  
-     __________________________________________________________________  
-  
    ### Selectlines  
+  
    selectlines shows all nonblank lines from the input  
    Example  
    cat file | selectlines  
    (echo 2; echo; echo; echo) | selectlines  
    => 2  
    The result would be 2, with no blank lines after that  
-     __________________________________________________________________  
-  
    ### Communicate  
+  
    Communicate is cool.  
    Communicate runs a Ruby expression after speaking a prompt (the first  
    argument) and getting your verbal answer (using something unfortunately  
    called “nerd-dictation”, which is a wrapper around another program  
    which deals with speech recognition)  
    Communicate allows you to have conversations with your computer, and it  
    is cross platform  
    (Or it hopefully is)  
    communicate 'What is the best color?' 'case text; when /blue/; puts  
    “You are right!”; when /red/; puts “Red is a bad color”; end '  
    That would be an example of how one could use “communicate”  
    Make sure you have nerd-dictation on your computer  
    The name nerd-dictation is absolutely awful, and I have to criticize  
    him for not making it have a better name, but it works.  
-     __________________________________________________________________  
+   ### Super Trans  
   
-   ### Super trans  
    super_trans is an offline translation program  
    It uses “Apertium”, which can do offline translation.  
    You can do translation anywhere with it.  
    It generates a webpage from the input text that not only has all  
    language translations embedded in it, it dynamically adjusts the  
    website page content to the web browser's “current language”.  
    You need to have a folder called “translation_folder” in your home  
@@ -403,55 +597,47 @@
    This is really powerful.  
    Some notes  
    This is worse than t.js in this software project  
    The resultant HTML is really big. It is too big.  
    “Automatic translation” is really powerful.  
    This translates into literally dozens of languages.  
    See also  
-   t.js  
-     __________________________________________________________________  
+        t.js  
+   ### To Buy Old  
   
-   ### To buy old  
    Old to buy tool, not that good  
-     __________________________________________________________________  
-  
    ### Executable  
-   Makes all the files in the current directory executable  
-     __________________________________________________________________  
   
+   Makes all the files in the current directory executable  
    ### Questions  
+  
    This program allows you to communicate with all important people in  
-   youife cycically and very easily. It's much easier than texting or  
+   your life cycically and very easily. It's much easier than texting or  
    normal emailing.  
+   It uses “email”, which currently doesn't work for Gmail.  
    See youtube.com/GregoryCohen1  
    See also  
-   tb (to buy)  
+        tb (to buy)  
    The youtube documentation video  
-     __________________________________________________________________  
-  
    ### Underline  
-   Underlines text  
-     __________________________________________________________________  
   
+   Underlines text  
    ### Processes  
+  
    Processes lists all processes with a certain name  
    For example  
    processes sh  
    processes bash  
    processes ruby  
    processes gsub  
-     __________________________________________________________________  
-  
    ### Emeraldc  
-   # EmeraldC  
+  
    The Ultimate C Preprocessor  
    I'm naming this preprocessor “Emerald C.”  
-   https://cboard.cprogramming.com/c-programming/181160-hi-i-have-created-  
-   some-work-i-think-will-really-valuable-community.html?s=589b5504cd0e3c2  
-   dc90e9abd8b66906f  
+   [17] Link  
    Howdy!  
    First, let me state that I am very much a perfectionist.  
    C is a wonderful language. C is probably the perfect programming  
    language. It is one of the top two most widely used languages for a  
    reason.  
    Now, there are some problems with it of course, but it's hard to think  
    of a more elegant language than it.  
@@ -465,27 +651,23 @@
    make another language. As a result, there are thousands of different  
    languages.  
    Well, recently, I made a preprocessor for C, that makes C incredibly  
    EASY.  
    C is fast and straightforward without it, but it has many features.  
    If one runs the command line preprocessor, with the “--features” flag,  
    the program shows all of its features  
-   --------------------------  
-  
-  A Better C  
-  
-   --------------------------  
+   A Better C  
    C is a fantastic language. C compiles insanely fast, is the fastest  
    language there is, is very clear, is native to all systems, and is  
    useful for all purposes.  
-   Some people, e.g., Bjarne Stroustrup, consider that C is "not good  
-   enough", and make languages like C++ or D (or thousands of others)  
+   Some people, e.g., Bjarne Stroustrup, consider that C is “not good  
+   enough”, and make languages like C++ or D (or thousands of others)  
    This is not necessary.  
-   There is no reason to use Python instead of C for "simple scripting  
-   tasks"  
+   There is no reason to use Python instead of C for “simple scripting  
+   tasks”  
    Some functions can be used as methods  
    Makes for an excellent “scripting language” (which is really just  
    native C without things making it slow)  
    1 String Interpolation “String interplation like this #{foo} ” Calls  
    the join() function (talked about below to join strings,  
    delim is a static global in each module called “sep”.  
    Make sure you free() the string after. The string is stored in a static  
@@ -501,17 +683,17 @@
    The preprocessor detects if you use and adds -lpcre2-8 to the link  
    flags if you use it. Use $" for substitutions in argument 3 gsub(a, b,  
    c)  
    8 join Joins an array of strings, to split(), use C's strtok (very  
    fast)  
    9 Lightweight regexes are added, almost 15 times as fast as C's built  
    in regex. They are very simple, they only have bracket expressions,  
-   like .  
+   like [a-z].  
    To use it, you need to pass a buffer of the size of the expansion of  
-   the regex. Foo would be Foo. That would be stored  
+   the regex. Foo[a-fA-F] would be Foo[abcdefABCDEF]. That would be stored  
    in a buffer.  
    From testing, 15x times faster than C's regex POST COMPILATION, if  
    compilation keeps happening, it might be hundreds of times faster.  
    Uses static inline functions, NO HEAP MEMORY unless you malloc  
    before().  
    10 print Like old python print “Hello” (fputs);  
    11 print_int prints a number and returns the number, can be chained  
@@ -524,21 +706,20 @@
    (frees str, sets to NULL, and frees other recent stuff)  
    asprintf() is another useful function which is UNIX-centric.  
    open_memstream() could be an alternative to std::string.  
    It works very well with each_line or by_lines (see above)  
    These features seem simple, but they can make C programming much, MUCH  
    easier  
    for example (insignificant example)  
-int main() {  
-    stdin.each_line { |line|  
-        print line;  
-    }  
-    free(line);  
-}  
-  
+   int main() {  
+   stdin.each_line { |line|  
+   print line;  
+   }  
+   free(line);  
+   }  
    You can iterate over the standard input like Ruby  
    The thing with this is that it has 100% speed. The resultant  
    preprocessed program becomes a normal C program  
    The compile and run time for a program (if you use tcc and not gcc) can  
    be about 24 milliseconds, which is faster than Ruby to run.  
    Even though the program is preprocessed, re-preprocessed, compiled,  
    assembled, linked, turned into an executable, and then run  
@@ -549,168 +730,148 @@
    else likes this work, and would like to use it, or to work with me.  
    Best regards,  
    Gregory  
    Current program is written in Crystal (crystal-lang.org) -- it was  
    written in ruby, it could be ported to another language.  
    I would like to make this self-hosting, but that would take a little  
    bit of work.  
-  
-About the Name  
-  
+   About the Name  
    Years ago, I really, really liked Compiz  
    Compiz then forked into Beryl. There was the Emerald Window Manager,  
    which was really nice and beautiful.  
    I actually made another programming language. I made 2 other  
    programming language. One was a full compiler and assembler, that ran  
    code in memory. It was around 16 thousand lines of code. I made a  
    programming language that had the syntax of Python or Ruby, but  
    transpiled into C++. I called that C += 2. I used that other language,  
-   and I created a Web Browser in it based on Chrome. I called it "Emerald  
-   Browser." Emeralds are beautiful green gems.  
-  
-   "Emerald is a gemstone and a variety of the mineral beryl colored green  
+   and I created a Web Browser in it based on Chrome. I called it “Emerald  
+   Browser.” Emeralds are beautiful green gems.  
+   “Emerald is a gemstone and a variety of the mineral beryl colored green  
    by trace amounts of chromium or sometimes vanadium. Beryl has a  
    hardness of 7.5–8 on the Mohs scale. Most emeralds are highly included,  
    so their toughness is classified as generally poor. Emerald is a  
-   cyclosilicate." --Wikipedia  
-  
+   cyclosilicate.”  
+   --Wikipedia  
    There was a browser with a terminal built in to it.  
    I show things off on my youtube channel, which I'm not going to link  
    here but is linked in my other repo.  
    This new language is better. It's ideal.  
-   ---  
    QUESTIONS  
-   ---  
    Why not use Rust?  
-$ time rustc a.rs  
-real    0m0.637s  
-user    0m0.502s  
-sys     0m0.160s  
-  
+   $ time rustc a.rs  
+   real 0m0.637s  
+   user 0m0.502s  
+   sys 0m0.160s  
    Rust takes 0.637 seconds to compile an empty file!  
    That is not ideal.  
-     __________________________________________________________________  
+   ### Last Nth  
   
-   ### Last nth  
    Last nth gets the last n lines from the standard input  
-     __________________________________________________________________  
-  
    ### Speakcat  
+  
    Speak cat is a tool like “cat”, which shows the content of files  
    (technically, it combines the content of files).  
    But speak cat also speaks the text.  
    Which could be useful in some circumstances.  
    It's kind of like “tee” to your ear.  
-     __________________________________________________________________  
+   ### Uca Cli  
   
-   ### Uca cli  
    CLI for uca app  
-     __________________________________________________________________  
+   ### Big Num  
   
-   ### Big num  
    big_num speaks really big numbers  
    Enter an expression, such as 2 ** 1000, and you'll see the result  
-     __________________________________________________________________  
-  
    ### Squeeze  
+  
    Squeeze is kind of like “sponge” from “moreutils”  
    But squeeze is different.  
    Squ  
    Squeeze reads all input, then it prints it back omitting argument 1  
    line from the front, and argument 2 lines from the back  
    Example  
    squeeze 1 1  
    This would omit the first line and the last line  
    squeeze 5 3  
    This would omit the first 5 lines and the last 3 lines  
-     __________________________________________________________________  
-  
    ### Foreach  
+  
    Reads a bunch of lines  
    Then a ruby expression is evaluated as the last line  
    The result is outputted in an argument.  
    You can enter /dev/null if you don't want an output file  
    “t” is better  
    See also  
-   t  
-     __________________________________________________________________  
-  
+        t  
    ### Dictate  
+  
    Dictate opens web pages in emerald browser, or in any browser  
    (depending on the environment variable set), by you speaking, instead  
    of typing.  
    There is a mode called c_mode, that allows you to make code from  
    speaking.  
-     __________________________________________________________________  
-  
    ### Prepend  
+  
    prepend prepends input taken from the standard input to a file  
    Usage  
-   prepend   
+   prepend [file]  
    This is text to be prepended  
-     __________________________________________________________________  
+   ### Chat Rb  
   
-   ### Chat rb  
    This program is excellent.  
    It's essentially a mix of ChatGPT and a shell, such as bash or ZSH.  
    It has a bunch of features.  
    It can display a file or change to a folder just by mentioning it.  
    It outputs chatgpt data to an output folder in home folder and copies  
    it to clipboard  
    To run a shell command, prefix things with “c”, such as c gcc.....  
-     __________________________________________________________________  
-  
    ### Undump  
+  
    undump is the opposite of dump  
    Example  
    echo cat | dump | undump  
    => cat  
    echo cat | dump  
    => “cat”  
    echo '“cat”' | undump  
    => cat  
-     __________________________________________________________________  
-  
    ### Append  
+  
    Appends text to file  
    Example  
    append file  
    This is more text to be appended  
-     __________________________________________________________________  
-  
    ### Email  
+  
+   ( This currently doesn't work for gmail since 2022 due to policy  
+   changes. :( )  
    A simple and practical tool to email people using Himalaya  
    Himalaya needs to be installed first  
    You would need to configure the script by changing its source code.  
    Modes  
-   email   
-   Email   
-   email   
+   email [no arguments]  
+   Email [yourself]  
+   email [addr]  
    Email one email address  
-   email     
+   email [Subject] [addr] [option more addrs]  
    Example  
    Email 'Gregory, I love your software!' gregorycohen2@gmail.com  
    my_friend@outlook.com person@example.com  
-     __________________________________________________________________  
-  
    ### Floor  
-   Gets the floor of numbers e.g. 21.3 -> 21  
-     __________________________________________________________________  
   
+   Gets the floor of numbers e.g. 21.3 -> 21  
    ### Query  
+  
    This is the top part of the job search, job search, etc. program for  
    Linux. The Linux program itself is called “linux_c_program”. The part  
    normally only works for Windows. This program works for Linux.  
-     __________________________________________________________________  
-  
    ### Lines  
-   Lines gets the number of files in the current folder that you are in.  
-     __________________________________________________________________  
   
+   Lines gets the number of files in the current folder that you are in.  
    ### Clock  
+  
    clock is useful  
    clock is a command line alarm clock  
    It wakes you up at 8:14, or at a time specified  
    Usage  
    clock  
    Runs clock  
    clock 15 30  
@@ -718,71 +879,37 @@
    clock 9 0  
    Sets an alarm clock for 9 in the morning  
    It uses flite to wake you up  
    It speaks with a bunch of voices  
    To stop it  
    Run this command  
    clock stop  
-     __________________________________________________________________  
-  
    ### Emoji  
+  
    Emoji converts words to emojis from the standard input  
    It can also speak the output  
    It can also copy the output to your clipboard  
    It is very useful  
-     __________________________________________________________________  
-  
    ### Close  
-   “Close” is a simple program that closes “Emerald Browser”, a new web  
-   browser based on the same engine as Chrome. Currently, Emerald Browser  
-   only works on Linux and Mac (Or Windows with Windows Subsystem for  
-   Linux or a Virtual Machine, but getting it to work might be tricky).  
-   “close” closes the Web Browser, which is normally full-screen.  
-   More accurately, it kills the browser, and all other copies of Emerald  
-   Browser.  
-   Since they are normally full screen, presumably the user would only  
-   have one instance of the browser open.  
-   The browser can have multiple panes (kind of like tabs) open, depending  
-   on how the browser is compiled.  
-   The browser can also be transparent, depending on how it is compiled.  
-   “Close” is supposed to be used in tandem with “open”, which is a  
-   command line tool to open the browser.  
-   open  ---->  gets searched in google, and then opened  
-   When you are done, you can do  
-   close  
-   Which closes the browser. It is a simple command.  
-   Currently, Emerald Browser is incomplete. A program exists in this  
-   software project that allows you to open up multiple browser tabs (one  
-   or more tabs) simply by speaking.  
-   Voice recognition would google the multiple sites that you say in your  
-   query (separated by “and”)  
-   “facebook and youtube and google”  
-   It's hard to get more direct than that!  
-   Emerald browser has a built in the top. The terminal is the navigation  
-   bar.  
-   Some more work needs to be put into the browser.  
-   Currently, new tabs can't be opened, which might be a dealbreaker for  
-   some people.  
-   Currently, content, like YouTube videos, can't be made fullscreen.  
-   If anyone wants to contribute, feel free to! :)  
-   “Close” is a simple program that closes “Emerald Browser”, a new web  
+  
+   “Close” is a simple program that closes “Emerald Browser,” a new web  
    browser based on the same engine as Chrome. Currently, Emerald Browser  
    only works on Linux and Mac (Or Windows with Windows Subsystem for  
    Linux or a Virtual Machine, but getting it to work might be tricky).  
    “close” closes the Web Browser, which is normally full-screen.  
    More accurately, it kills the browser, and all other copies of Emerald  
    Browser.  
    Since they are normally full screen, presumably the user would only  
    have one instance of the browser open.  
    The browser can have multiple panes (kind of like tabs) open, depending  
    on how the browser is compiled.  
    The browser can also be transparent, depending on how it is compiled.  
-   “Close” is supposed to be used in tandem with “open”, which is a  
+   “Close” is supposed to be used in tandem with “open,” which is a  
    command line tool to open the browser.  
-   open  ---->  gets searched in google, and then opened  
+   open [query] ----> [query] gets searched in google, and then opened  
    When you are done, you can do  
    close  
    Which closes the browser. It is a simple command.  
    Currently, Emerald Browser is incomplete. A program exists in this  
    software project that allows you to open up multiple browser tabs (one  
    or more tabs) simply by speaking.  
    Voice recognition would google the multiple sites that you say in your  
@@ -791,132 +918,126 @@
    It's hard to get more direct than that!  
    Emerald browser has a built in the top. The terminal is the navigation  
    bar.  
    Some more work needs to be put into the browser.  
    Currently, new tabs can't be opened, which might be a dealbreaker for  
    some people.  
    Currently, content, like YouTube videos, can't be made fullscreen.  
-   If anyone wants to contribute, feel free to! :)  
-     __________________________________________________________________  
-  
+   If anyone wants to contribute, feel free to! 🙂  
    ### Copy  
+  
    copy copies the standard input  
    Example  
    ls | copy  
-     __________________________________________________________________  
-  
    ### Gsub  
+  
    Gsub is very powerful.  
    Usage  
-   gsub    
+   gsub [regular expression] [replacement text]  
    Example  
    cat text | gsub man dog  
    cat text | gsub 'man|boy|cat|dog' food  
    ls | gsub Desktop cat  
-     __________________________________________________________________  
+   ### News  
   
+   Gets the news from bbc  
+   Usage  
+   news  
+   news speak  
+   uses google_speak to SPEAK the news, one story at a time.  
+   🙂  
    ### Dump  
+  
    Dump surrounds its input with quotes  
    ls | dump  
    => “....”  
    Use undump to get the reverse  
    See also  
-   undump  
-     __________________________________________________________________  
-  
+        undump  
    ### Bold  
-   See other color programs  
-     __________________________________________________________________  
   
+   See other color programs  
    ### Args  
+  
    args is like a better xargs  
    args works properly with spaces in the name of commands  
    It takes exactly one argument  
    Example  
    ls | args “mv -t ../f”  
-     __________________________________________________________________  
-  
    ### Open  
+  
    “open” is a very efficient program that searches a query from google,  
    and then opens it in Emerald Browser.  
    If you ever want something to “just open”, you can use it.  
    Example  
    open “cats”  
    An earlier version of open worked like this  
-   open    N  
+   open [site1] [site2] [site3] N  
    site1, site2, and site3 would all be opened, and the top N queries were  
    all shown in different panes  
    An even earlier version of this program used Chrome to open the sites.  
    The current version can open one or more sites.  
    Example  
    open “cats” “dogs” “frogs”  
    All of those queries would open in Emerald Browser.  
    Just make sure it is compiled in multipane mode if you want to open  
    multiple new sites at the same time.  
    See also  
-   emerald-browser  
+        emerald-browser  
    close  
-     __________________________________________________________________  
-  
    ### Swap  
-   Swaps two files  
-     __________________________________________________________________  
   
+   Swaps two files  
    ### Exp  
+  
    exp is an exponentiation tool  
    (echo 5; echo 3) | exp  
    => 125  
    (echo 2; echo 10) | exp  
    => 1024  
-     __________________________________________________________________  
-  
    ### Div  
+  
    Div divides integers  
    Example  
    (echo 5000; echo 100)|div  
    => 50  
-     __________________________________________________________________  
-  
    ### Mul  
+  
    Multiply numbers  
    echo 1 > file  
    echo 2 > file  
    echo 3 > file  
    echo 4 > file  
    echo 5 > file  
    cat file | mul  
    => 120  
-     __________________________________________________________________  
-  
    ### Nth  
-   Nth gets the nth line from the input  
-     __________________________________________________________________  
   
+   Nth gets the nth line from the input  
    ### Abs  
+  
    Abs gets the absolute value of an integer  
    The absolute value of a number is the value of that number without its  
    sign  
    echo -300 | abs  
    => 300  
    echo 200 | abs  
    => 200  
    (echo -2; echo -10) | sub | abs  
    => 12  
    The last one would do -2 - -10, the result would be -12, and then the  
    absolute value would be computed, and so the result would be 12.  
-     __________________________________________________________________  
-  
    ### Add  
+  
    See the sub example  
    add adds integers from the standard input  
    (echo 1; echo 2; echo 3) | add  
    The result would be 6  
-     __________________________________________________________________  
-  
    ### Sub  
+  
    Sub is a simple command line program that subtracts integers.  
    For some reason, no simple program did this.  
    Which is weird  
    Example  
    sub  
    (Input)  
    10  
@@ -924,29 +1045,26 @@
    1  
    Result =>  
    6  
    Example  
    (echo 5; echo 2) | sub  
    Result =>  
    3  
-     __________________________________________________________________  
-  
    ### G+  
+  
    A compiler for C += 2  
    Usage is like g++  
    Example  
    g+ a.cpp -o out  
    See also README file & emerald-browser and its source  
-     __________________________________________________________________  
-  
    ### Tb  
-   SEE THIS YOUTUBE CHANNEL AND SUBSCRIBE  
-     __________________________________________________________________  
   
+   [18] SEE THIS YOUTUBE CHANNEL AND SUBSCRIBE  
    ### T  
+  
    “t” is incredibly useful.  
    It can be used many, many times every day by computer power users.  
    It is kind of like “sed”, or perl, python or ruby.  
    It's the ULTIMATE shell “glue” tool.  
    t reads every line from the standard input, and for every line, it  
    evaluates a ruby expression  
    t a + 2  
@@ -968,18 +1086,30 @@
    cat /usr/share/dict/words | t 'a + “ is a good word.”'  
    That processes every word in the dictionary, and says that every word  
    “is a good word.”  
    There are other programs in this software project like “t”.  
    But if you do command line text filtering, t might be the best tool  
    that you will find.  
    See also  
-   gsub  
+        gsub  
    gsub_in_place  
   
 References  
   
    1. https://www.youtube.com/GregoryCohen1  
    2. https://facebook.com/democracygregoryc  
    3. mailto:gregorycohen@gmail.com  
-   4. http://www.github.com/gregoryc/democracy  
-   5. http://www.rubygems.org/gems/democracy  
-   6. http://www.youtube.com/GregoryCohen1  
+   4. https://pypi.org/project/democracy  
+   5. https://www.rubygems.org/gem/democracy  
+   6. https://www.linkedin.com/in/gregory-cohen-274333261/  
+   7. https://www.youtube.com/GregoryCohen1  
+   8. https://facebook.com/democracygregoryc  
+   9. https://www.rubygems.org/gems/computers  
+  10. https://www.rubygems.org/gems/democracy  
+  11. https://www.rubygems.org/gems/linux  
+  12. https://www.rubygems.org/gems/string  
+  13. https://www.rubygems.org/gems/unix  
+  14. http://www.github.com/gregoryc/democracy  
+  15. http://www.rubygems.org/gems/democracy  
+  16. https://pypi.org/project/democracy  
+  17. “https://cboard.cprogramming.com/c-programming/181160-hi-i-have-created-some-work-i-think-will-really-valuable-community.html?s=589b5504cd0e3c2dc90e9abd8b66906f”  
+  18. http://www.youtube.com/GregoryCohen1
```

### Comparing `democracy-1.0.22/pyproject.toml` & `democracy-1.0.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "democracy"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.22"  # Required
+version = "1.0.23"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Trying to help with democracy, see https://github.com/gregoryc/democracy"  # Optional
 
 # This is an optional longer description of your project that represents
```

