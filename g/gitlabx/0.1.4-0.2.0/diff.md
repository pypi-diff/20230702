# Comparing `tmp/gitlabx-0.1.4-py3-none-any.whl.zip` & `tmp/gitlabx-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,19 @@
-Zip file size: 8218 bytes, number of entries: 16
+Zip file size: 8866 bytes, number of entries: 17
+-rwxrwxrwx  2.0 unx      970 b- defN 23-Jul-02 21:49 gitlabx/Member.py
 -rwxrwxrwx  2.0 unx        0 b- defN 23-Jun-28 23:28 gitlabx/__init__.py
 -rwxrwxrwx  2.0 unx      380 b- defN 23-Jun-29 10:14 gitlabx/abstract.py
--rwxrwxrwx  2.0 unx      953 b- defN 23-Jun-29 11:24 gitlabx/branches.py
--rwxrwxrwx  2.0 unx      963 b- defN 23-Jun-29 11:24 gitlabx/commits.py
+-rwxrwxrwx  2.0 unx      950 b- defN 23-Jun-29 23:39 gitlabx/branches.py
+-rwxrwxrwx  2.0 unx      972 b- defN 23-Jun-30 00:06 gitlabx/commits.py
 -rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/deployments.py
 -rwxrwxrwx  2.0 unx      902 b- defN 23-Jun-29 11:24 gitlabx/events.py
--rwxrwxrwx  2.0 unx     1801 b- defN 23-Jun-29 11:12 gitlabx/factories.py
+-rwxrwxrwx  2.0 unx     1985 b- defN 23-Jul-02 21:49 gitlabx/factories.py
 -rwxrwxrwx  2.0 unx      944 b- defN 23-Jun-29 11:24 gitlabx/issues.py
 -rwxrwxrwx  2.0 unx      785 b- defN 23-Jun-29 11:24 gitlabx/project.py
 -rwxrwxrwx  2.0 unx      979 b- defN 23-Jun-29 11:24 gitlabx/projectLanguages.py
 -rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/repositories.py
 -rwxrwxrwx  2.0 unx     1080 b- defN 23-Jun-29 11:24 gitlabx/repositoryTree.py
--rwxrwxrwx  2.0 unx     1675 b- defN 23-Jun-29 11:29 gitlabx-0.1.4.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-29 11:29 gitlabx-0.1.4.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-29 11:29 gitlabx-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1215 b- defN 23-Jun-29 11:29 gitlabx-0.1.4.dist-info/RECORD
-16 files, 13829 bytes uncompressed, 6236 bytes compressed:  54.9%
+-rwxrwxrwx  2.0 unx     1675 b- defN 23-Jul-02 21:51 gitlabx-0.2.0.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-02 21:51 gitlabx-0.2.0.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-02 21:51 gitlabx-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Jul-02 21:51 gitlabx-0.2.0.dist-info/RECORD
+17 files, 15062 bytes uncompressed, 6774 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: gitlabx/Member.py
+Comment: 
+
 Filename: gitlabx/__init__.py
 Comment: 
 
 Filename: gitlabx/abstract.py
 Comment: 
 
 Filename: gitlabx/branches.py
@@ -30,20 +33,20 @@
 
 Filename: gitlabx/repositories.py
 Comment: 
 
 Filename: gitlabx/repositoryTree.py
 Comment: 
 
-Filename: gitlabx-0.1.4.dist-info/METADATA
+Filename: gitlabx-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: gitlabx-0.1.4.dist-info/WHEEL
+Filename: gitlabx-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: gitlabx-0.1.4.dist-info/top_level.txt
+Filename: gitlabx-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gitlabx-0.1.4.dist-info/RECORD
+Filename: gitlabx-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitlabx/branches.py

```diff
@@ -17,15 +17,15 @@
 			logging.info("Start function: get_Branches")
 			result = self.gl.projects.list(owned=True, iterator=True)
 			for project in result:
 				branches = project.branches.list()
 				project = project.asdict()
 				for	branch in branches:
 					branch = branch.asdict()
-					branch['project_id'] = project['id']
+					branch['project'] = project['id']
 					branch_list.append(branch)
 			
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__) 
 
 		logging.info("Retrieve All Project Branches")
```

## gitlabx/commits.py

```diff
@@ -15,15 +15,15 @@
 		commit_list = []
 
 		try:
 			logging.info("Start function: get_Commits")
 			result = self.gl.projects.list(owned=True, iterator=True)
 
 			for project in result:
-				commits = project.commits.list(iterator=True)
+				commits = project.commits.list(iterator=True,all=True)
 				project = project.asdict()
 				for	commit in commits:
 					commit = commit.asdict()
 					commit['project_id'] = project['id']
 					commit_list.append(commit)
 			
 		except Exception as e:
```

## gitlabx/factories.py

```diff
@@ -4,22 +4,31 @@
 from .branches import Branches
 from .commits import Commits
 from .deployments import Deployments
 from .events import Events
 from .issues import Issues
 from .repositories import Repositories
 from .projectLanguages import ProjectLanguages
+from .Member import Member
 
 class ProjectFactory(factory.Factory):
     
     class Meta:
         model = Project
         
     personal_access_token = None
     gitlab_url = None
+
+class MembersFactory(factory.Factory):
+    
+    class Meta:
+        model = Member
+        
+    personal_access_token = None
+    gitlab_url = None
   
 class RepositoryTreeFactory(factory.Factory):
     
     class Meta:
         model = RepositoryTree
         
     personal_access_token = None
```

## Comparing `gitlabx-0.1.4.dist-info/METADATA` & `gitlabx-0.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabx
-Version: 0.1.4
+Version: 0.2.0
 Summary: Uma Lib para buscar dados do Gitlab
 Home-page: https://gitlab.com/immigrant-data-driven-development/libs/application/gitlab
 Author: Carlos Henrique Maulaz de Freitas
 Author-email: carlosmaulaz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gitlabx-0.1.4.dist-info/RECORD` & `gitlabx-0.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+gitlabx/Member.py,sha256=c79PUpvZJQ4WrergPIZQoBf_SdUm3OlPye7BXSwrAPk,970
 gitlabx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gitlabx/abstract.py,sha256=mc5cmcD-klDfmHwo0HSl8itgsAiHx9nla1d5FQFjmcQ,380
-gitlabx/branches.py,sha256=kf1GLkt4SxaZ_LhgBD6RpqQb1w8HepyYTe7l4XahhD0,953
-gitlabx/commits.py,sha256=7WRYLatBxVM5P0ljjaMgj8Ay44NinlFmvhEKryEUkek,963
+gitlabx/branches.py,sha256=HRgOYKxRQbjYDo50ZbwqbgvC5qxyLKEzsKC4nF8Zyw8,950
+gitlabx/commits.py,sha256=vvPc5RiN079bgLk2uBb3EfwjpuPmlZtvVzcdGAWeqnQ,972
 gitlabx/deployments.py,sha256=sa8S9wmox-8ihRLwZq1mvpxKU5N8iKK0S7W8R1L11Q8,1026
 gitlabx/events.py,sha256=Nl6q0E3mc_x_XFlyGDNLj1m8Z5iieLiKfMs1HEvZTIY,902
-gitlabx/factories.py,sha256=nFQIQg6VSTiEUOZb2_52OwRqJqyD5jEGHWCTTXWKUbM,1801
+gitlabx/factories.py,sha256=KCDpxJ4hEEtTmhUVigxJr2ezhcQkxA5R6I92YvdBIXQ,1985
 gitlabx/issues.py,sha256=WRiKt2Oz23quLD_8RoFCZfZwfxiYgRBs7N19DxFtDSw,944
 gitlabx/project.py,sha256=28QdSWWM0swGkFC9LeCZW5mAXobXp02UKNZYEIhky50,785
 gitlabx/projectLanguages.py,sha256=qhRf543cotBVMdAlkaZ_CW9KU1y9e2Pxyw6Vsj4zkls,979
 gitlabx/repositories.py,sha256=o5p06Cf_x1hXmltKiecFvWO1MyQyX5L6jLy-He0_sgs,1026
 gitlabx/repositoryTree.py,sha256=lmdEdLucR4FaUWZtVy1z3R2TFzY6cwYtfJ4OeZ6j8JU,1080
-gitlabx-0.1.4.dist-info/METADATA,sha256=2765Dd1Wq7Ox7yWdbZ63DjNkmWpVpjXyduQGIq_uYB8,1675
-gitlabx-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gitlabx-0.1.4.dist-info/top_level.txt,sha256=EkmcO7CZ14bNE_fgl8kFTFfgu1K7yvMO481rj0zu6ns,8
-gitlabx-0.1.4.dist-info/RECORD,,
+gitlabx-0.2.0.dist-info/METADATA,sha256=hd-iO5X-cdjPqr2WxaA8_ZSmYU7KnSBpnh6dq-N351M,1675
+gitlabx-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gitlabx-0.2.0.dist-info/top_level.txt,sha256=EkmcO7CZ14bNE_fgl8kFTFfgu1K7yvMO481rj0zu6ns,8
+gitlabx-0.2.0.dist-info/RECORD,,
```

