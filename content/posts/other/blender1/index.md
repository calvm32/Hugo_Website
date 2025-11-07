---
title: "Blender Mesh"
description: "How to make meshes in the newest version of blender"
menu:
  sidebar:
    name: Blender Mesh
    identifier: blender_mesh
    parent: other
    weight: 1
hero: bg.png
date: 2025-11-06T08:06:25+06:00
---

Recently, I wanted to make a fun mesh, which meant I needed Blender, Gmsh, and two Blender add-ons called <a href="">blendmsh</a> and <a href="https://www.blenderkit.com/">Blender Kit</a>.

This post is about blendmsh, which is a great bridge between Blender and Gmsh (which itself is a bridge to actually running simulations). Unfortunately, blendmsh is not compatible with Blender versions 4.0 and greater, so one needs to make the following changes to 

<code> Application Support/Blender/4.5/scripts/addons/blendmsh-master/utils_pip.py </code>:

<ol>
  <li style="color: #E5EAC3;"> At the start of the file, include <code> import sys </code> to access paths based on the current run, which avoids dealing with versions. </li>
  <li style="color: #E5EAC3;"> In one of the following lines, replace whichever <code> PYPATH </code> is given with <code> PYPATH = sys.executable </code> </li>
  <li style="color: #E5EAC3;"> Finally, the second argument of <code> bpy.utils.user_resource </code> has apparently become keyword-only, so simply writing <code> "site-package" </code> is invalid. Instead, this entire line should be replaced with 
  
  <code> site_package = bpy.utils.user_resource('SCRIPTS', path="site_package", create=True) </code>. </li>
</ol>