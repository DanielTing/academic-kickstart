---
# Display name
name: Daniel Ting

# Username (this should match the folder name)
authors:
- admin

# Is this the primary user of the site?
superuser: true

# Role/position
role: Staff Research Scientist

# Organizations/Affiliations
organizations:
- name: Tableau Research
  url: "https://research.tableau.com/user/daniel-ting"

# Short bio (displayed in user profile at end of posts)
bio: My recent research focuses on data sketching and sampling. These techniques drastically reduce the size of Big Data and allow users to extract approximate answers from in-memory summaries that are constructed in one-pass over the original data.

interests:
- Data sketching
- Experimentation
- Manifold Learning
- Artificial Intelligence

education:
  courses:
  - course: PhD in Statistics with designated emphasis in ML
    institution: University of California, Berkeley
    year: 2012
  - course: MS in Statistics
    institution: Carnegie Mellon
    year: 2006
  - course: BS in Computer Science and Math
    institution: Carnegie Mellon
    year: 2002

# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/widgets/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- icon: envelope
  icon_pack: fas
  link: '#contact'  # For a direct email link, use "mailto:test@example.org".
#- icon: twitter
#  icon_pack: fab
#  link: https://twitter.com/GeorgeCushen
- icon: google-scholar
  icon_pack: ai
  link: https://scholar.google.com/citations?user=KxDB5bAAAAAJ
#- icon: github
#  icon_pack: fab
#  link: https://github.com/gcushen
# Link to a PDF of your resume/CV from the About widget.
# To enable, copy your resume/CV to `static/files/cv.pdf` and uncomment the lines below.  
# - icon: cv
#   icon_pack: ai
#   link: files/cv.pdf

# Enter email to display Gravatar (if Gravatar enabled in Config)
email: ""
  
# Organizational groups that you belong to (for People widget)
#   Set this to `[]` or comment out if you are not using People widget.  
# user_groups:
# - Researchers
# - Visitors
---

My research is in statistics, databases, and machine learning. In particular, my recent work is primarily on the topic of data sketching. These are techniques for approximate query processing where a stream of Big Data is compressed into a small memory summary that can be queried quickly and provide answers to a range of questions. It lies in the intersection of statistics, databases, and algorithms. 

I received my PhD in Statistics at UC Berkeley under the supervision of Michael Jordan. My PhD work focused on non-parametric Bayesian cluster models and semi-supervised/manifold learning. I continue to work on manifold learning. I also worked on data privacy for my MSc at Carnegie Mellon under Stephen Fienberg. Before Tableau, I was a core data scientist at Facebook where I helped start and build the experiment analysis platform.

This site is partly meant to make my work more accessible to data sketching practitioners and the underlying principles behind it clearer to researchers. While I have always tried to leverage my industry experience to address practical problems that practitioners face, the research papers themselves can sometimes be hard to digest, or the simple parts are hard to separate from the more complex parts. I have also found that my theoretical statistics background brings unique perspectives and techniques to the field of data sketching, much of which has been developed by the good work of the theoretical CS community. My hope is that the adoption of some of these techniques can further the field of data sketching.
