# Comparing `tmp/iam_ape-1.1.3.tar.gz` & `tmp/iam_ape-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_ape-1.1.3.tar", max compression
+gzip compressed data, was "iam_ape-1.1.4.tar", max compression
```

## Comparing `iam_ape-1.1.3.tar` & `iam_ape-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-27 15:26:26.770889 iam_ape-1.1.3/LICENSE
--rw-r--r--   0        0        0     3031 2023-04-27 15:26:26.771008 iam_ape-1.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771631 iam_ape-1.1.3/iam_ape/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 15:26:26.771725 iam_ape-1.1.3/iam_ape/aws_iam_actions/__init__.py
--rw-r--r--   0        0        0   261088 2023-05-15 10:16:11.384423 iam_ape-1.1.3/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
--rw-r--r--   0        0        0     2854 2023-05-15 10:16:11.386023 iam_ape-1.1.3/iam_ape/aws_iam_actions/scrape_iam_actions.py
--rw-r--r--   0        0        0     1748 2023-05-10 17:34:00.350992 iam_ape-1.1.3/iam_ape/consts.py
--rw-r--r--   0        0        0    31189 2023-06-06 14:28:48.009240 iam_ape-1.1.3/iam_ape/evaluator.py
--rw-r--r--   0        0        0    15833 2023-05-15 10:16:11.386516 iam_ape-1.1.3/iam_ape/expand_policy.py
--rw-r--r--   0        0        0     3435 2023-06-06 14:28:48.009997 iam_ape-1.1.3/iam_ape/helper_classes.py
--rw-r--r--   0        0        0     7808 2023-06-06 14:28:48.010292 iam_ape-1.1.3/iam_ape/helper_functions.py
--rw-r--r--   0        0        0     1224 2023-04-27 15:26:26.773011 iam_ape-1.1.3/iam_ape/helper_types.py
--rw-r--r--   0        0        0     9999 2023-05-10 17:34:00.351593 iam_ape-1.1.3/iam_ape/main.py
--rw-r--r--   0        0        0        0 2023-04-27 15:26:26.773181 iam_ape-1.1.3/iam_ape/py.typed
--rw-r--r--   0        0        0     1257 2023-06-06 14:28:48.010532 iam_ape-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     4279 1970-01-01 00:00:00.000000 iam_ape-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-21 14:09:32.879473 iam_ape-1.1.4/LICENSE
+-rw-r--r--   0        0        0     3031 2023-04-27 15:10:48.767861 iam_ape-1.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-03-21 14:09:32.880346 iam_ape-1.1.4/iam_ape/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-21 14:09:32.880510 iam_ape-1.1.4/iam_ape/aws_iam_actions/__init__.py
+-rw-r--r--   0        0        0   268029 2023-07-02 13:55:02.077670 iam_ape-1.1.4/iam_ape/aws_iam_actions/aws_iam_actions.tar.gz
+-rw-r--r--   0        0        0     2854 2023-06-14 12:54:53.805389 iam_ape-1.1.4/iam_ape/aws_iam_actions/scrape_iam_actions.py
+-rw-r--r--   0        0        0     1748 2023-06-14 12:54:41.874913 iam_ape-1.1.4/iam_ape/consts.py
+-rw-r--r--   0        0        0    31608 2023-07-02 14:27:23.113324 iam_ape-1.1.4/iam_ape/evaluator.py
+-rw-r--r--   0        0        0     1356 2023-07-02 14:25:16.249010 iam_ape-1.1.4/iam_ape/exceptions.py
+-rw-r--r--   0        0        0    17383 2023-07-02 14:25:16.244940 iam_ape-1.1.4/iam_ape/expand_policy.py
+-rw-r--r--   0        0        0     3850 2023-07-02 13:55:49.184117 iam_ape-1.1.4/iam_ape/helper_classes.py
+-rw-r--r--   0        0        0     8484 2023-07-02 14:27:23.102561 iam_ape-1.1.4/iam_ape/helper_functions.py
+-rw-r--r--   0        0        0     1224 2023-04-27 15:10:48.770874 iam_ape-1.1.4/iam_ape/helper_types.py
+-rw-r--r--   0        0        0    10177 2023-07-02 14:27:23.111139 iam_ape-1.1.4/iam_ape/main.py
+-rw-r--r--   0        0        0        0 2023-03-23 15:18:42.495823 iam_ape-1.1.4/iam_ape/py.typed
+-rw-r--r--   0        0        0     1257 2023-07-02 13:59:25.712463 iam_ape-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4231 1970-01-01 00:00:00.000000 iam_ape-1.1.4/PKG-INFO
```

### Comparing `iam_ape-1.1.3/LICENSE` & `iam_ape-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.3/README.md` & `iam_ape-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.3/iam_ape/aws_iam_actions/scrape_iam_actions.py` & `iam_ape-1.1.4/iam_ape/aws_iam_actions/scrape_iam_actions.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.3/iam_ape/consts.py` & `iam_ape-1.1.4/iam_ape/consts.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.3/iam_ape/evaluator.py` & `iam_ape-1.1.4/iam_ape/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import json
 import logging
 from collections import defaultdict
 from dataclasses import replace
-from fnmatch import fnmatch
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple
 
 from iam_ape.consts import PolicyElement
+from iam_ape.exceptions import EntityNotFoundException, PolicyNotFoundException
 from iam_ape.expand_policy import PolicyExpander
 from iam_ape.helper_classes import (
     Action,
     IneffectiveAction,
     PermissionsContainer,
     PolicyWithSource,
 )
 from iam_ape.helper_functions import (
     deep_update,
     get_default_policy_for_managed_policy,
     merge_condition,
     normalize_policy,
+    wildcard_match,
 )
 from iam_ape.helper_types import EntityType, FinalReportT
 
 logger = logging.getLogger("IAM-APE:evaluator")
 
 
 def should_deny(
@@ -49,15 +50,15 @@
                             not_resource=None,
                             condition=merge_condition(
                                 iam_action.condition, denied_action.condition
                             ),
                             source=iam_action.source,
                         )
                     )
-                elif fnmatch(
+                elif wildcard_match(
                     iam_action.resource, denied_action.resource
                 ):  # denied Resource > allowed Resource
                     if not denied_action.condition:
                         return True, set(), denied_action.source
                     partially_denied = True
                     res.add(
                         Action(
@@ -66,15 +67,15 @@
                             not_resource=None,
                             condition=merge_condition(
                                 iam_action.condition, denied_action.condition
                             ),
                             source=iam_action.source,
                         )
                     )
-                elif fnmatch(
+                elif wildcard_match(
                     denied_action.resource, iam_action.resource
                 ):  # allowed Resource > denied Resource
                     partially_denied = True
                     res.add(
                         Action(
                             action=iam_action.action,
                             resource=None
@@ -102,19 +103,19 @@
                             source=iam_action.source,
                         )
                     )
 
             if denied_action.not_resource:
                 if denied_action.not_resource == iam_action.resource:
                     pass
-                elif fnmatch(
+                elif wildcard_match(
                     iam_action.resource, denied_action.not_resource
                 ):  # denied NotResource > allowed Resource
                     pass
-                elif fnmatch(
+                elif wildcard_match(
                     denied_action.not_resource, iam_action.resource
                 ):  # denied NotResource < allowed Resource
                     partially_denied = True
                     res.add(
                         Action(
                             action=iam_action.action,
                             resource=denied_action.not_resource,
@@ -127,19 +128,19 @@
                     )
 
         if iam_action.not_resource:
 
             if denied_action.resource:
                 if denied_action.resource == iam_action.not_resource:
                     pass
-                elif fnmatch(
+                elif wildcard_match(
                     denied_action.resource, iam_action.not_resource
                 ):  # allowed NotResource > denied Resource
                     pass
-                elif fnmatch(
+                elif wildcard_match(
                     iam_action.not_resource, denied_action.resource
                 ):  # denied Resource > allowed NotResource
                     partially_denied = True
                     res.add(
                         Action(
                             action=iam_action.action,
                             resource=iam_action.resource,
@@ -176,19 +177,19 @@
                             not_resource=iam_action.not_resource,
                             condition=merge_condition(
                                 iam_action.condition, denied_action.condition
                             ),
                             source=iam_action.source,
                         )
                     )
-                elif fnmatch(
+                elif wildcard_match(
                     denied_action.not_resource, iam_action.not_resource
                 ):  # allowed NotResource > denied NotResource
                     pass
-                elif fnmatch(
+                elif wildcard_match(
                     iam_action.not_resource, denied_action.not_resource
                 ):  # denied NotResource > allowed NotResource
                     partially_denied = True
                     res.add(
                         Action(
                             action=iam_action.action,
                             resource=iam_action.resource,
@@ -269,15 +270,15 @@
         if permission_boundary.allowed_permissions:
             for values in permission_boundary.allowed_permissions.values():
                 for value in values:
                     return value.source
         for values in permission_boundary.denied_permissions.values():
             for value in values:
                 return value.source
-        raise ValueError("Permission Boundary source not found")
+        raise PolicyNotFoundException("Permission Boundary source not found")
 
     permission_boundary_id = get_pb_id()
 
     new_allow_actions = defaultdict(set)
     ineffective_permissions: Set[IneffectiveAction] = set()
     for action_key, action_values in allow_actions.items():
         if action_key not in permission_boundary.allowed_permissions.keys():
@@ -296,19 +297,23 @@
                 ]:
 
                     if action_tuple.resource and boundary_tuple.resource:
                         if action_tuple.resource == boundary_tuple.resource:
                             new_allow_actions[action_key].add(
                                 permit(action_tuple, boundary_tuple)
                             )  # action is permitted
-                        elif fnmatch(action_tuple.resource, boundary_tuple.resource):
+                        elif wildcard_match(
+                            action_tuple.resource, boundary_tuple.resource
+                        ):
                             new_allow_actions[action_key].add(
                                 permit(action_tuple, boundary_tuple)
                             )  # action is permitted
-                        elif fnmatch(boundary_tuple.resource, action_tuple.resource):
+                        elif wildcard_match(
+                            boundary_tuple.resource, action_tuple.resource
+                        ):
                             new_allow_actions[action_key].add(
                                 replace(
                                     action_tuple,
                                     resource=boundary_tuple.resource,
                                     condition=merge_condition(
                                         action_tuple.condition,
                                         boundary_tuple.condition,
@@ -324,21 +329,21 @@
                     elif action_tuple.resource and boundary_tuple.not_resource:
                         if (
                             action_tuple.resource == boundary_tuple.not_resource
                         ):  # action is not permitted
                             ineffective_permissions.add(
                                 deny(action_tuple, permission_boundary_id)
                             )
-                        elif fnmatch(
+                        elif wildcard_match(
                             action_tuple.resource, boundary_tuple.not_resource
                         ):  # action is not permitted
                             ineffective_permissions.add(
                                 deny(action_tuple, permission_boundary_id)
                             )
-                        elif fnmatch(
+                        elif wildcard_match(
                             boundary_tuple.not_resource, action_tuple.resource
                         ):  # action is partially permitted
                             new_allow_actions[action_key].add(
                                 replace(
                                     action_tuple,
                                     not_resource=boundary_tuple.not_resource,
                                     condition=merge_condition(
@@ -356,29 +361,29 @@
                     elif action_tuple.not_resource and boundary_tuple.resource:
                         if (
                             action_tuple.not_resource == boundary_tuple.resource
                         ):  # action is not permitted
                             ineffective_permissions.add(
                                 deny(action_tuple, permission_boundary_id)
                             )
-                        elif fnmatch(
+                        elif wildcard_match(
                             action_tuple.not_resource, boundary_tuple.resource
                         ):  # action is partially permitted
                             new_allow_actions[action_key].add(
                                 replace(
                                     action_tuple,
                                     resource=boundary_tuple.resource,
                                     condition=merge_condition(
                                         action_tuple.condition,
                                         boundary_tuple.condition,
                                         negate=False,
                                     ),
                                 )
                             )
-                        elif fnmatch(
+                        elif wildcard_match(
                             boundary_tuple.resource, action_tuple.not_resource
                         ):  # action is not permitted
                             ineffective_permissions.add(
                                 deny(action_tuple, permission_boundary_id)
                             )
                         else:  # action is partially permitted
                             new_allow_actions[action_key].add(
@@ -397,24 +402,24 @@
                     elif action_tuple.not_resource and boundary_tuple.not_resource:
                         if (
                             action_tuple.not_resource == boundary_tuple.resource
                         ):  # action is permitted
                             new_allow_actions[action_key].add(
                                 permit(action_tuple, boundary_tuple)
                             )
-                        elif fnmatch(
+                        elif wildcard_match(
                             action_tuple.not_resource, boundary_tuple.not_resource
                         ):  # action is partially permitted
                             new_allow_actions[action_key].add(
                                 replace(
                                     action_tuple,
                                     not_resource=boundary_tuple.not_resource,
                                 )
                             )
-                        elif fnmatch(
+                        elif wildcard_match(
                             boundary_tuple.not_resource, action_tuple.not_resource
                         ):  # action is permitted
                             new_allow_actions[action_key].add(
                                 permit(action_tuple, boundary_tuple)
                             )
                         else:  # action is partially permitted
                             new_allow_actions[action_key].add(
@@ -449,15 +454,16 @@
     ineffective_permissions.update(denied_ineffective)
     return allowed, ineffective_permissions
 
 
 class AuthorizationDetails(object):
     def __init__(self, auth_report: Optional[Dict[str, Any]] = None):
         if auth_report is None:
-            raise ValueError("Could not load account authorization details")
+            logger.error("Could not load account authorization details")
+            auth_report = {}
 
         self.User: Dict[str, Any] = {
             user["Arn"]: user for user in auth_report.get("UserDetailList", [])
         }
         self.Group: Dict[str, Any] = {
             group["Arn"]: group for group in auth_report.get("GroupDetailList", [])
         }
@@ -640,18 +646,19 @@
         return None
 
     def get_managed_policies(
         self, managed_policies: List[Dict[str, str]]
     ) -> Iterator[PolicyWithSource]:
         for policy_details in managed_policies:
             policy_arn = policy_details["PolicyArn"]
-            policy = get_default_policy_for_managed_policy(
-                self.auth_details.Policy.get(policy_arn, {})
-            )
-            yield PolicyWithSource(policy=policy, source=policy_arn)
+            if policy_obj := self.auth_details.Policy.get(policy_arn):
+                policy = get_default_policy_for_managed_policy(policy_obj)
+                yield PolicyWithSource(policy=policy, source=policy_arn)
+            else:
+                PolicyNotFoundException(f"Couldn't find policy {policy_arn}")
 
     def get_permission_boundary(self, entity: Dict[str, Any]) -> PermissionsContainer:
         permissions = PermissionsContainer()
         if pb_arn := entity.get("PermissionsBoundary", {}).get(
             "PermissionsBoundaryArn"
         ):
             policy = PolicyWithSource(
@@ -665,15 +672,15 @@
 
         return permissions
 
     def evaluate(self, arn: str, entity_type: EntityType) -> PermissionsContainer:
         entity_obj = getattr(self.auth_details, entity_type.value).get(arn)
         if not entity_obj:
             logger.error(f"Error - couldn't find entity with ARN {arn}")
-            raise ValueError(f"couldn't find entity with ARN {arn}")
+            raise EntityNotFoundException(arn)
 
         direct_policies = self.get_direct_policies(entity_obj, entity_type)
         indirect_policies: List[PolicyWithSource] = []
         if entity_type == EntityType.user:
             for group in entity_obj.get("GroupList", []):
                 group_obj = self.get_group_object_by_name(group)
                 if group_obj:
```

### Comparing `iam_ape-1.1.3/iam_ape/expand_policy.py` & `iam_ape-1.1.4/iam_ape/expand_policy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,75 @@
+import functools
 import json
 import logging
+import re
 import tarfile
 from collections import defaultdict
 from fnmatch import fnmatch
 from typing import Any, Dict, FrozenSet, List, Literal, Optional, Set, Tuple
 
 from requests.structures import CaseInsensitiveDict
 
 from iam_ape.consts import RESOURCE_ARN_RE, PolicyElement, actions_json_location
+from iam_ape.exceptions import UnknownServiceExepction
 from iam_ape.helper_classes import (
     Action,
     HashableDict,
     HashableList,
     PermissionsContainer,
     PolicyWithSource,
 )
-from iam_ape.helper_functions import as_list, normalize_policy
+from iam_ape.helper_functions import as_list, normalize_policy, wildcard_match
 from iam_ape.helper_types import AwsPolicyStatementType, AwsPolicyType
 
 logger = logging.getLogger("policy expander")
+WORDSPLIT_RE = re.compile(r"(?<=.)(?=[A-Z])")
+
+
+class FrozenSetSet:
+    pass
+
+
+@functools.lru_cache()
+def shorten_to_leading_word(actions: FrozenSet[str]) -> Dict[str, Set[str]]:
+    """
+    Shorten a list of actions to their leading word,
+    e.g. ['DescribeInstances', 'DescribeVolumes'] -> {'Describe': ['DescribeInstances', 'DescribeVolumes']}
+    :param actions: list of actions
+    :returns: dict of leading words to actions
+    """
+    action_mapping = defaultdict(set)
+    for action in actions:
+        action_words = WORDSPLIT_RE.split(action)
+        action_mapping[action_words[0]].add(action)
+    return action_mapping
+
+
+def minimize_actions(
+    service: str, actions: List[str], all_iam_actions: List[str]
+) -> List[str]:
+    """
+    Minimize a list of actions for a given service, by replacing a list of actions with a wildcard if possible.
+    :param service: service name
+    :param actions: list of actions
+    :return: a list of actions
+    """
+    if len(actions) == 1:
+        return [f"{service}:{actions[0]}"]
+    if len(actions) == len(all_iam_actions):
+        return [f"{service}:*"]
+    all_service_wildcards = shorten_to_leading_word(frozenset(all_iam_actions))
+    statements_wildcards = shorten_to_leading_word(frozenset(actions))
+    res = []
+    for wildcard, used_actions in statements_wildcards.items():
+        if len(used_actions) == len(all_service_wildcards[wildcard]):
+            res.append(f"{service}:{wildcard}*")
+        else:
+            res.extend([f"{service}:{action}" for action in used_actions])
+    return res
 
 
 def _append_action(
     res: Dict[str, Set[Action]],
     action: str,
     service: str,
     resources: Optional[List[str]],
@@ -224,15 +271,15 @@
         else:  # {"NotAction": ["ec2:*", "iam:Get*", "sts:GetCallerIdentity"]}
             for iam_service, action_dicts in self.all_iam_actions.items():
                 for action in action_dicts.keys():
                     curr_action = f"{iam_service}:{action}"
                     curr_action_lower = curr_action.lower()
                     if any(
                         [
-                            fnmatch(curr_action_lower, not_action.lower())
+                            wildcard_match(curr_action_lower, not_action.lower())
                             for not_action in notactions
                         ]
                     ):
                         continue
                     _append_action(
                         res=res,
                         action=curr_action,
@@ -254,35 +301,34 @@
         policy_statements: List[AwsPolicyStatementType],
     ) -> List[AwsPolicyStatementType]:
         for statement in policy_statements:
             action_dict = defaultdict(list)
             for action in statement.get(PolicyElement.ACTION) or []:
                 service, action_key = action.split(":", maxsplit=1)
                 action_dict[service].append(action_key)
+            statement_actions = []
             for service, action_keys in action_dict.items():
-                try:
-                    if all(
-                        [
-                            action in action_keys
-                            for action in self.all_iam_actions[service]
-                        ]
-                    ):
-                        for action_key in action_keys:
-                            statement[PolicyElement.ACTION].remove(f"{service}:{action_key}")  # type: ignore
-                        statement[PolicyElement.ACTION].append(f"{service}:*")  # type: ignore
-                except KeyError as e:
-                    logger.exception(f"Unknown service: {service=}")
-                    raise e
+                if all_service_actions := self.all_iam_actions.get(service):
+                    statement_actions.extend(
+                        minimize_actions(
+                            service=service,
+                            actions=action_keys,
+                            all_iam_actions=all_service_actions,
+                        )
+                    )
+                else:
+                    raise UnknownServiceExepction(service)
             if all(
                 [
-                    action in as_list(statement[PolicyElement.ACTION])
+                    action in as_list(statement_actions)
                     for action in self._all_service_wildcards
                 ]
             ):
-                statement[PolicyElement.ACTION] = ["*"]
+                statement_actions = ["*"]
+            statement[PolicyElement.ACTION] = statement_actions
         return policy_statements
 
     def shrink_policy(self, allow_actions: Dict[str, Set[Action]]) -> AwsPolicyType:
         policy_res: AwsPolicyType = {"Statement": []}
         squashed_policies: Set[Action] = set()
         for allow_action_set in allow_actions.values():
             squashed_policies.update(allow_action_set)
```

### Comparing `iam_ape-1.1.3/iam_ape/helper_classes.py` & `iam_ape-1.1.4/iam_ape/helper_classes.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,27 @@
     AwsPolicyType,
     IneffectiveActionDict,
     PermissionsContainerDict,
 )
 
 
 class HashableList(list):
+    def __init__(self, lst: list) -> None:
+        super().__init__()
+        for item in lst:
+            if isinstance(item, dict):
+                self.append(HashableDict.recursively(item))
+            elif isinstance(item, list):
+                self.append(HashableList(item))
+            else:
+                assert hasattr(item, "__hash__"), f"Unhashable type: {type(item)}"
+                self.append(item)
+
     def __hash__(self) -> int:  # type: ignore[override]
-        return hash(tuple(sorted(self)))
+        return hash(frozenset(self))
 
 
 class HashableDict(dict):
     def __hash__(self) -> int:  # type: ignore[override]
         return hash(tuple(sorted(self.items())))
 
     @classmethod
```

### Comparing `iam_ape-1.1.3/iam_ape/helper_functions.py` & `iam_ape-1.1.4/iam_ape/helper_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
+from fnmatch import fnmatch
 from typing import Any, Dict, List, Literal, Optional, Set, TypeVar
 
-from iam_ape.consts import CONDITIONS_NEGATIONS
+from iam_ape.consts import CONDITIONS_NEGATIONS, PolicyElement
+from iam_ape.exceptions import MalformedPolicyDocumentException, PolicyNotFoundException
 from iam_ape.helper_classes import HashableDict, HashableList
 from iam_ape.helper_types import AwsPolicyType
 
 logger = logging.getLogger(__name__)
 
 KeyType = TypeVar("KeyType")
 
@@ -15,17 +17,17 @@
         return []
     if isinstance(element, list):
         return element
     return [element]
 
 
 def normalize_policy(policy: AwsPolicyType) -> AwsPolicyType:
-    def verify_type(subject: Any, subject_type: Any, err_msg: str) -> None:
+    def verify_type(subject: Any, subject_type: Any) -> None:
         if not isinstance(subject, subject_type):
-            raise TypeError(err_msg)
+            raise MalformedPolicyDocumentException(subject_type, type(subject).__name__)
 
     def normalize_dict(
         dict_to_norm: Dict[str, Any], fields: Optional[Set[str]] = None
     ) -> Dict[str, Any]:
         for field in fields or set(dict_to_norm.keys()):
             if not isinstance(dict_to_norm.get(field, []), list):
                 dict_to_norm[field] = [dict_to_norm[field]]
@@ -42,31 +44,38 @@
     }
     aws_statement_action_keys: Set[Literal["Action", "NotAction"]] = {
         "Action",
         "NotAction",
     }
 
     if not isinstance(policy, dict):
-        raise TypeError(f"Malformed policy. Expected dict, got: {type(policy)}")
+        raise MalformedPolicyDocumentException(dict, type(policy).__name__)
 
     for field in aws_policy_str_fields:
         verify_type(
             policy.get(field, ""),
             str,
-            err_msg=f"Malformed Policy, expected {field} of type str",
         )
 
     policy = normalize_dict(policy, aws_policy_list_fields)  # type: ignore
 
     for statement in policy["Statement"]:
         verify_type(
-            statement["Effect"],
+            statement[PolicyElement.EFFECT],
             str,
-            err_msg="Malformed Policy, expected statement Effect of type str",
         )
+        if not statement[PolicyElement.EFFECT] in ["Allow", "Deny"]:
+            if statement[PolicyElement.EFFECT].lower() == "deny":
+                statement[PolicyElement.EFFECT] = "Deny"
+            elif statement[PolicyElement.EFFECT].lower() == "allow":
+                statement[PolicyElement.EFFECT] = "Allow"
+            else:
+                raise MalformedPolicyDocumentException(
+                    "Allow or Deny", statement[PolicyElement.EFFECT]
+                )
 
         # Normalize list fields
         statement = normalize_dict(statement, aws_statement_list_fields)  # type: ignore
 
         # Normalize Principal and NotPrincipal to look like this:
         # {"Statement":
         #   {"Principal":
@@ -79,37 +88,39 @@
             if not statement.get(field):
                 continue
             if statement[field] == "*":  # type: ignore
                 statement[field] = {"AWS": ["*"]}  # type: ignore
             verify_type(
                 statement.get(field, {}),
                 dict,
-                err_msg=f"Malformed Policy, expected {field} of type dict",
             )
             statement[field] = normalize_dict(statement[field])  # type: ignore
 
         # Normalize Condition to look like this:
         # {
         #   Statement: {
         #     Condition: {
         #       ConditionOperator: {
         #           ConditionKey: [ConditionValue]
         #       }
         #     }
         #   }
         # }
         verify_type(
-            statement.get("Condition", {}),
+            statement.get(PolicyElement.CONDITION, {}),
             dict,
-            err_msg="Malformed Policy, expected Condition of type dict",
         )
-        for condition_operator, condition_dict in statement.get("Condition", {}).items():  # type: ignore
+        for condition_operator, condition_dict in statement.get(PolicyElement.CONDITION, {}).items():  # type: ignore
             for condition_key, condition_value in condition_dict.items():
                 if not isinstance(condition_value, list):
-                    statement["Condition"][condition_operator][condition_key] = [condition_value]  # type: ignore
+                    statement[PolicyElement.CONDITION][condition_operator][  # type: ignore
+                        condition_key
+                    ] = [
+                        condition_value
+                    ]
 
         for action_key in aws_statement_action_keys:
             if action_list := statement.get(action_key):
                 new_action_list = []
                 for action in action_list:
                     if action.count(":") == 1:
                         service, action_name = action.split(":")
@@ -194,15 +205,15 @@
 
 def get_default_policy_for_managed_policy(
     managed_policy_obj: Dict[str, Any]
 ) -> AwsPolicyType:
     for policy in managed_policy_obj.get("PolicyVersionList", []):
         if policy.get("IsDefaultVersion", False):
             return normalize_policy(policy["Document"])
-    raise ValueError(
+    raise PolicyNotFoundException(
         f"No default policy found for managed policy {managed_policy_obj['Arn']}"
     )
 
 
 def deep_update(
     mapping: Dict[KeyType, Any], *updating_mappings: Dict[KeyType, Any]
 ) -> Dict[KeyType, Any]:
@@ -213,7 +224,15 @@
                 if isinstance(updated_mapping[k], dict) and isinstance(v, dict):
                     updated_mapping[k] = deep_update(updated_mapping[k], v)
                 elif isinstance(updated_mapping[k], list) and isinstance(v, list):
                     updated_mapping[k] = list(set(updated_mapping[k] + v))
             else:
                 updated_mapping[k] = v
     return updated_mapping
+
+
+def wildcard_match(s: str, pattern: str) -> bool:
+    if pattern == "*":
+        return True
+    if "*" in pattern:
+        return fnmatch(s, pattern)
+    return s == pattern
```

### Comparing `iam_ape-1.1.3/iam_ape/helper_types.py` & `iam_ape-1.1.4/iam_ape/helper_types.py`

 * *Files identical despite different names*

### Comparing `iam_ape-1.1.3/iam_ape/main.py` & `iam_ape-1.1.4/iam_ape/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import boto3
 from botocore.exceptions import ClientError, ProfileNotFound
 
 from iam_ape.aws_iam_actions.scrape_iam_actions import scrape_iam_actions
 from iam_ape.evaluator import AuthorizationDetails, EffectivePolicyEvaluator
+from iam_ape.exceptions import (
+    AwsAuthorizationException,
+    IamApeException,
+    InvalidArnException,
+)
 from iam_ape.helper_classes import PolicyWithSource
 from iam_ape.helper_functions import deep_update
 from iam_ape.helper_types import AwsPolicyType, EntityType, FinalReportT
 
 logger = logging.getLogger("IAM-APE")
 logging.getLogger("botocore").setLevel(logging.WARNING)  # suppress botocore logs
-entity_regex_string = r"arn:aws(-cn|-us-gov)?:iam::(?P<account>\d{12}):(?P<entity_type>user|group|role)/[\w-]+"
+entity_regex_string = r"arn:aws(-cn|-us-gov)?:iam::(?P<account>\d{12}):(?P<entity_type>user|group|role)(?P<path>(/[a-zA-Z0-9+=,.@_-]+)*)?/[a-zA-Z0-9+=,.@_-]+"  # noqa: E501
 entity_regex = re.compile(entity_regex_string)
 
 banner = """
   __   __   _  _        __   ____  ____ 
  (  ) / _\ ( \/ ) ___  / _\ (  _ \(  __)
   )( /    \/ \/ \(___)/    \ ) __/ ) _) 
  (__)\_/\_/\_)(_/     \_/\_/(__)  (____)
@@ -69,17 +74,15 @@
 
 
 def validate_arn(arn: str) -> Tuple[EntityType, str]:
     regex_match = entity_regex.fullmatch(arn)
     try:
         assert regex_match
     except AssertionError:
-        raise ValueError(
-            f'Invalid ARN format: "{arn}". Expected: "{entity_regex_string}"'
-        )
+        raise InvalidArnException(arn, entity_regex_string)
 
     entity_type = regex_match.group("entity_type")
     account_id = regex_match.group("account")
 
     if entity_type == "user":
         return EntityType.user, account_id
     elif entity_type == "group":
@@ -104,15 +107,15 @@
     elif (
         not profile
         and os.environ.get("AWS_ACCESS_KEY_ID")
         and os.environ.get("AWS_SECRET_ACCESS_KEY")
     ):
         logger.info("AWS Auth: Using environment variables")
     else:
-        raise ValueError(
+        raise AwsAuthorizationException(
             "AWS Auth: No authentication method found. "
             "Please set AWS_PROFILE (or use --profile) or AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY"
         )
     iam_client = boto3.client("iam")
     paginator = iam_client.get_paginator("get_account_authorization_details")
     for page in paginator.paginate():
         auth_report = deep_update(auth_report, page)
@@ -133,15 +136,15 @@
     account_id: str, profile: Optional[str] = None
 ) -> List[PolicyWithSource]:
     logger.info("Attempting to fetch service control policies from AWS...")
     profile = profile or os.environ.get("AWS_PROFILE")
     policies = []
 
     if not profile:
-        raise ValueError("No AWS profile found")
+        raise AwsAuthorizationException("No AWS profile found")
 
     boto3.setup_default_session(profile_name=profile)
     org_client = boto3.client("organizations")
     paginator = org_client.get_paginator("list_policies_for_target")
 
     for page in paginator.paginate(
         TargetId=account_id, Filter="SERVICE_CONTROL_POLICY"
@@ -270,21 +273,21 @@
     if arguments.update:
         scrape_iam_actions()
         if not arguments.arn:
             return 0
 
     try:
         entity_type, entity_account = validate_arn(arguments.arn)
-    except ValueError as e:
+    except InvalidArnException as e:
         logger.error(e)
         return -1
 
     try:
         auth_details = get_auth_details(arguments.input, arguments.profile)
-    except (ValueError, ProfileNotFound) as e:
+    except (AwsAuthorizationException, ProfileNotFound) as e:
         logger.error(e)
         return -1
 
     scp_policies = None
     if arguments.input is None or arguments.scp_policy is not None:
         scp_policies = get_scp_policies(
             arguments.scp_policy, arguments.profile, entity_account
@@ -293,15 +296,15 @@
     logger.info("Evaluating effective permissions")
     calculator = EffectivePolicyEvaluator(
         authorization_details=auth_details, scp_policies=scp_policies
     )
 
     try:
         res = calculator.evaluate(arn=arguments.arn, entity_type=entity_type)
-    except ValueError as e:
+    except IamApeException as e:
         logger.error(e)
         return -1
 
     out: Union[AwsPolicyType, FinalReportT]
     if arguments.format == "clean":
         out = calculator.policy_expander.shrink_policy(res.allowed_permissions)
     else:
```

### Comparing `iam_ape-1.1.3/pyproject.toml` & `iam_ape-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-ape"
-version = "1.1.3"
+version = "1.1.4"
 description = "IAM AWS Permissions Evaluator"
 authors = ["Tohar Braun, Orca Security <tohar@orca.security>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 repository = "https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/"
 keywords = ["aws", "iam"]
```

### Comparing `iam_ape-1.1.3/PKG-INFO` & `iam_ape-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-ape
-Version: 1.1.3
+Version: 1.1.4
 Summary: IAM AWS Permissions Evaluator
 Home-page: https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/
 License: GPL-3.0-or-later
 Keywords: aws,iam
 Author: Tohar Braun, Orca Security
 Author-email: tohar@orca.security
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,14 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Requires-Dist: beautifulsoup4 (>=4.8.2,<5.0.0)
 Requires-Dist: boto3 (>=1.24.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: tqdm (>=4.63.0,<5.0.0)
 Project-URL: Repository, https://github.com/orcasecurity/orca-toolbox/raw/main/iam-ape/
 Description-Content-Type: text/markdown
```

