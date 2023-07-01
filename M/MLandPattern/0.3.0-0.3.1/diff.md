# Comparing `tmp/MLandPattern-0.3.0.tar.gz` & `tmp/MLandPattern-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.3.0.tar", last modified: Mon Jun 26 17:26:30 2023, max compression
+gzip compressed data, was "MLandPattern-0.3.1.tar", last modified: Sat Jul  1 23:37:16 2023, max compression
```

## Comparing `MLandPattern-0.3.0.tar` & `MLandPattern-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 17:26:30.975237 MLandPattern-0.3.0/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 17:26:30.971963 MLandPattern-0.3.0/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)    28961 2023-06-26 17:25:46.000000 MLandPattern-0.3.0/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.3.0/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-26 17:26:30.974218 MLandPattern-0.3.0/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-26 17:26:30.000000 MLandPattern-0.3.0/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-26 17:26:30.000000 MLandPattern-0.3.0/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-26 17:26:30.000000 MLandPattern-0.3.0/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-26 17:26:30.000000 MLandPattern-0.3.0/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-26 17:26:30.974793 MLandPattern-0.3.0/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.3.0/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-26 17:26:30.975406 MLandPattern-0.3.0/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-26 17:01:01.000000 MLandPattern-0.3.0/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-07-01 23:37:16.119485 MLandPattern-0.3.1/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-07-01 23:37:16.116091 MLandPattern-0.3.1/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)    36705 2023-07-01 23:36:18.000000 MLandPattern-0.3.1/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.3.1/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-07-01 23:37:16.118506 MLandPattern-0.3.1/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-07-01 23:37:16.000000 MLandPattern-0.3.1/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-07-01 23:37:16.000000 MLandPattern-0.3.1/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-07-01 23:37:16.000000 MLandPattern-0.3.1/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-07-01 23:37:16.000000 MLandPattern-0.3.1/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-07-01 23:37:16.119122 MLandPattern-0.3.1/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.3.1/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-07-01 23:37:16.119651 MLandPattern-0.3.1/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-07-01 23:36:27.000000 MLandPattern-0.3.1/setup.py
```

### Comparing `MLandPattern-0.3.0/MLandPattern/MLandPattern.py` & `MLandPattern-0.3.1/MLandPattern/MLandPattern.py`

 * *Files 13% similar despite different names*

```diff
@@ -496,22 +496,20 @@
     :return acc: Accuracy of the validation set
     """
     class_labels = np.unique(train_labels)
     with_cov = covariance_within_class(train_data, train_labels)
     multi_mu = multiclass_mean(train_data, train_labels)
     densities = []
     for i in range(class_labels.size):
-        densities.append(
-            np.exp(logLikelihood(test_data, vcol(multi_mu[i, :]), with_cov))
-        )
+        densities.append(logLikelihood(test_data, vcol(multi_mu[i, :]), with_cov))
     S = np.array(densities)
-
-    SJoint = S * prior_probability
-    SMarginal = vrow(SJoint.sum(0))
-    SPost = SJoint / SMarginal
+    logSJoint = S + np.log(prior_probability)
+    logSMarginal = vrow(scipy.special.logsumexp(logSJoint, axis=0))
+    logSPost = logSJoint - logSMarginal
+    SPost = np.exp(logSPost)
     predictions = np.argmax(SPost, axis=0)
 
     if len(test_label) != 0:
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
@@ -539,19 +537,20 @@
     class_labels = np.unique(train_labels)
     cov = covariance_within_class(train_data, train_labels)
     identity = np.eye(cov.shape[1])
     cov = cov * identity
     multi_mu = multiclass_mean(train_data, train_labels)
     densities = []
     for i in range(class_labels.size):
-        densities.append(np.exp(logLikelihood(test_data, vcol(multi_mu[i, :]), cov)))
+        densities.append(logLikelihood(test_data, vcol(multi_mu[i, :]), cov))
     S = np.array(densities)
-    SJoint = S * prior_probability
-    SMarginal = vrow(SJoint.sum(0))
-    SPost = SJoint / SMarginal
+    logSJoint = S + np.log(prior_probability)
+    logSMarginal = vrow(scipy.special.logsumexp(logSJoint, axis=0))
+    logSPost = logSJoint - logSMarginal
+    SPost = np.exp(logSPost)
     predictions = np.argmax(SPost, axis=0)
 
     if len(test_label) != 0:
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
@@ -598,26 +597,32 @@
         [Probabilities, Prediction, accuracy] = Tied_Naive_classifier(
             train_attributes, train_labels, test_attributes, prior_prob, test_labels
         )
         accuracy = round(accuracy * 100, 2)
     return Probabilities, Prediction, accuracy
 
 
-def k_fold(k, attributes, labels, previous_prob, model="mvg", PCA_m=0, LDA_m=0):
+def k_fold(
+    k, attributes, labels, previous_prob, model="mvg", PCA_m=0, LDA_m=0, l=0.001
+):
     """
     Applies a k-fold cross validation on the dataset, applying the specified model.
     :param: `k` Number of partitions to divide the dataset
     :param: `attributes` matrix containing the whole training attributes of the dataset
     :param: `labels` the label vector related to the attribute matrix
     :param: `previous_prob` the column vector related to the prior probability of the dataset
     :param: `model` (optional). Defines the model to be applied to the model:
         - `mvg`: Multivariate Gaussian Model
         - `Naive`: Naive Bayes Classifier
         - `Tied Gaussian`: Tied Multivariate Gaussian Model
         - `Tied naive`: Tied Naive Bayes Classifier
+        - `Regression` : Binomial Regression
+    :param: `PCA_m` (optional) a number of dimensions to reduce using PCA method
+    :param: `LDA_m` (optional) a number of dimensions to reduce using LDA mehtod
+    :param: `l` (optional) hyperparameter to use when the method is linera regression, default value set to 0.001
     :return final_acc: Accuracy of the validation set
     :return final_S: matrix associated with the probability array
     """
     section_size = int(attributes.shape[1] / k)
     cont = 0
     low = 0
     high = section_size
@@ -632,24 +637,30 @@
             if PCA_m:
                 P, train_att = PCA(train_att, PCA_m)
                 validation_att = np.dot(P.T, validation_att)
                 if LDA_m:
                     W, _ = LDA1(train_att, train_labels, LDA_m)
                     train_att = np.dot(W.T, train_att)
                     validation_att = np.dot(W.T, validation_att)
-            [S, _, acc] = Generative_models(
-                train_att,
-                train_labels,
-                validation_att,
-                previous_prob,
-                validation_labels,
-                model,
-            )
+            if model == "regression":
+                [S, prediction, acc] = binaryRegression(
+                    train_att, train_labels, l, validation_att, validation_labels
+                )
+            else:
+                [S, prediction, acc] = Generative_models(
+                    train_att,
+                    train_labels,
+                    validation_att,
+                    previous_prob,
+                    validation_labels,
+                    model,
+                )
             final_acc = acc
             final_S = S
+            final_prediction = prediction
             continue
         low += section_size
         high += section_size
         if high > attributes.shape[1]:
             high = attributes.shape
         validation_att = attributes[:, low:high]
         validation_labels = labels[low:high]
@@ -660,44 +671,49 @@
         if PCA_m:
             P, train_att = PCA(train_att, PCA_m)
             validation_att = np.dot(P.T, validation_att)
             if LDA_m:
                 W, _ = LDA1(train_att, train_labels, LDA_m)
                 train_att = np.dot(W.T, train_att)
                 validation_att = np.dot(W.T, validation_att)
-        [S, _, acc] = Generative_models(
-            train_att,
-            train_labels,
-            validation_att,
-            previous_prob,
-            validation_labels,
-            model,
-        )
+        if model == "regression":
+            [S, prediction, acc] = binaryRegression(
+                train_att, train_labels, l, validation_att, validation_labels
+            )
+        else:
+            [S, prediction, acc] = Generative_models(
+                train_att,
+                train_labels,
+                validation_att,
+                previous_prob,
+                validation_labels,
+                model,
+            )
         final_acc += acc
         final_S += S
     final_acc /= k
     final_S /= k
-    return final_acc, final_S
+    return final_S, prediction, final_acc
+
 
 def logreg_obj(v, DTR, LTR, l):
     """
     Method to calculate the error of a function based on the data points
     :param v: Vector of the values to evaluate [w, b]
     :param DTR: Matrix with all the train attributes
     :param LTR: Matrix with all the train labels
     :param l: Hyperparameter l to apply to the function
     :return: retFunc the value of evaluating the function on the input parameter v
     """
     n = DTR.shape[1]
     w, b = v[0:-1], v[-1]
     log_sum = 0
-    for i in range(n):
-        zi = 1 if LTR[i] else -1
-        inter_sol = -zi * (np.dot(w.T, DTR[:, i]) + b)
-        log_sum += np.logaddexp(0, inter_sol)
+    zi = LTR * 2 - 1
+    inter_sol = -zi * (np.dot(w.T, DTR) + b)
+    log_sum = np.sum(np.logaddexp(0, inter_sol))
     retFunc = l / 2 * np.power(np.linalg.norm(w), 2) + 1 / n * log_sum
     return retFunc
 
 
 def binaryRegression(train_attributes, train_labels, l, test_attributes, test_labels):
     """
     Method to calculate the error of a function based on the data points
@@ -719,8 +735,225 @@
     funct = lambda s: 1 if s > 0 else 0
     predictions = np.array(list(map(funct, S)))
     acc = 0
     for i in range(test_labels.shape[0]):
         if predictions[i] == test_labels[i]:
             acc += 1
     acc /= test_labels.size
-    return w, S, acc
+    acc = round(acc * 100, 2)
+
+    return w, S, acc
+
+
+def polynomial_kernel(xi, xj, d, C, eps):
+    interm = np.dot(xi.T, xj)
+    interm += C
+    G = np.power(interm, d) + eps
+    return G
+
+
+def radial_kernel(xi, xj, gamma, eps):
+    diff = xi[:, :, np.newaxis] - xj[:, np.newaxis, :]
+    G = -gamma * np.square(np.linalg.norm(diff, axis=0))
+    G = np.add(np.exp(G), eps)
+    return G
+
+
+def dual_svm(
+    alpha,
+    training_att,
+    training_labels,
+    K=1,
+    d=0,
+    c=0,
+    eps=0,
+    gamma=0,
+    funct="polynomial",
+):
+    kern = funct.lower()
+    one = np.ones(training_att.shape[1])
+    zi = 2 * training_labels - 1
+    if kern == "polynomial":
+        G = polynomial_kernel(training_att, training_att, d, c, eps)
+    elif kern == "radial":
+        G = radial_kernel(training_att, training_att, gamma, eps=eps)
+    else:
+        D = np.vstack((training_att, one * K))
+        G = np.dot(D.T, D)
+    z = np.outer(zi, zi)
+    H = np.multiply(z, G)
+    retFun = np.dot(alpha.T, H)
+    retFun = np.dot(retFun, alpha) / 2
+    retFun = retFun - np.dot(alpha.T, one)
+    retGrad = np.dot(H, alpha)
+    retGrad -= one
+    return (retFun, retGrad)
+
+
+def svm(
+    training_att,
+    training_labels,
+    test_att,
+    test_labels,
+    constrain,
+    model="",
+    dim=2,
+    c=1,
+    K=1,
+    gamma=1,
+    eps=0,
+):
+    """
+    Apply the Support Vector Machine model, using either one of the models described to approximate the soluction.
+    :param train_att: Matrix with all the train attributes
+    :param train_labels: Matrix with all the train labels
+    :param test_att: Matrix with all the train attributes
+    :param test_labels: Matrix with all the train labels
+    :param constrain: Constrain of maximum value of the alpha vector
+    :param model: (optional) define the applied kernel model:
+    - `polynomial`: polynomial kernel of degree d
+    - `Radial`: Radial Basis Function kernel
+    - Default: leave empty, and the dual SVM method is applied
+    :param dim: (optional) hyperparameter for polynomial method. `Default 2`
+    :param c: (optional) hyperparameter for polynomial method. `Default 1`
+    :param K: (optional) hyperparameter for dual SVM method. `Default 1`
+    :param gamma: (optional) hyperparameter for radial method. `Default 1`
+    :param eps: (optional) hyperparameter for kernel methods. `Default 0`
+    """
+    alp = np.ones(training_att.shape[1])
+    constrain = np.array([(0, constrain)] * training_att.shape[1])
+    [x, f, d] = scipy.optimize.fmin_l_bfgs_b(
+        dual_svm,
+        alp,
+        args=(training_att, training_labels, K, dim, c, eps, gamma, model),
+        bounds=constrain,
+    )
+    print(d["nit"])
+    zi = 2 * training_labels - 1
+    kern = model.lower()
+    if kern == "polynomial":
+        S = x * zi
+        S = np.dot(S, polynomial_kernel(training_att, test_att, dim, c, eps))
+    elif kern == "radial":
+        S = x * zi
+        S = np.dot(S, radial_kernel(training_att, test_att, gamma, eps))
+    else:
+        D = np.ones(training_att.shape[1]) * K
+        D = np.vstack((training_att, D))
+        w = x * zi
+        w = w * D
+        w = np.sum(w, axis=1)
+        x_val = np.vstack((test_att, np.ones(test_att.shape[1]) * K))
+        S = np.dot(w.T, x_val)
+    # funct = lambda s: 1 if s > 0 else 0
+    predictions = np.where(S > 0, 1, 0)
+    error = np.abs(predictions - test_labels)
+    error = np.sum(error)
+    error /= test_labels.size
+
+    return S, predictions, 1 - error
+
+
+def calculate_model(S, test_points, model, prior_probability, test_labels=[]):
+    model = model.lower()
+    funct = lambda s: 1 if s > 0 else 0
+    if model == "Generative":
+        logSJoint = S + np.log(prior_probability)
+        logSMarginal = vrow(scipy.special.logsumexp(logSJoint, axis=0))
+        logSPost = logSJoint - logSMarginal
+        SPost = np.exp(logSPost)
+        predictions = np.argmax(SPost, axis=0)
+    elif model == "regression":
+        predictions = np.array(list(map(funct, S)))
+    else:
+        predictions = np.array(list(map(funct, S)))
+    if len(test_labels) != 0:
+        error = np.abs(test_labels - predictions)
+        error = np.sum(error)
+    return predictions, (1 - error)
+
+
+def ConfMat(predicted, actual):
+    labels = np.unique(np.concatenate((actual, predicted)))
+
+    matrix = np.zeros((len(labels), len(labels)), dtype=int)
+
+    for true_label, predicted_label in zip(actual, predicted):
+        true_index = np.where(labels == true_label)[0]
+        predicted_index = np.where(labels == predicted_label)[0]
+        matrix[predicted_index, true_index] += 1
+
+    return matrix
+
+
+def OptimalBayes(llr, labels, pi, Cfn, Cfp):
+    log_odds = llr
+    threshold = -np.log((pi * Cfn) / ((1 - pi) * Cfp))
+    decisions = np.where(log_odds > threshold, 1, 0)
+
+    tp = np.sum(np.logical_and(decisions == 1, labels == 1))
+    fp = np.sum(np.logical_and(decisions == 1, labels == 0))
+    tn = np.sum(np.logical_and(decisions == 0, labels == 0))
+    fn = np.sum(np.logical_and(decisions == 0, labels == 1))
+
+    confusion_matrix = np.array([[tn, fn], [fp, tp]])
+
+    return confusion_matrix
+
+
+def Bayes_risk(confusion_matrix, pi, Cfn, Cfp):
+    M01 = confusion_matrix[0][1]
+    M11 = confusion_matrix[1][1]
+    M10 = confusion_matrix[1][0]
+    M00 = confusion_matrix[0][0]
+
+    FNR = M01 / (M01 + M11)
+    FPR = M10 / (M00 + M10)
+
+    DCF = pi * Cfn * FNR + (1 - pi) * Cfp * FPR
+
+    B = min(pi * Cfn, (1 - pi) * Cfp)
+
+    DCFnorm = DCF / B
+
+    return DCF, round(DCFnorm, 2)
+
+
+def minCostBayes(llr, labels, pi, Cfn, Cfp):
+    if llr.ndim > 1:
+        llr = (Cfn * llr[0, :]) / (Cfp * llr[1, :])
+    sortedLLR = np.sort(llr)
+    # sortedLLR = pi * sortedLLR[0, :] / ((1 - pi) * sortedLLR[1, :])
+    t = np.array([-np.inf, np.inf])
+    t = np.append(t, sortedLLR)
+    t = np.sort(t)
+    DCFnorm = []
+    FNRlist = []
+    FPRlist = []
+    for i in t:
+        threshold = i
+        funct = lambda s: 1 if s > i else 0
+        decisions = np.array(list(map(funct, llr)))
+        # decisions = np.where(llr > threshold, 1, 0)
+
+        tp = np.sum(np.logical_and(decisions == 1, labels == 1))
+        fp = np.sum(np.logical_and(decisions == 1, labels == 0))
+        tn = np.sum(np.logical_and(decisions == 0, labels == 0))
+        fn = np.sum(np.logical_and(decisions == 0, labels == 1))
+
+        confusion_matrix = np.array([[tn, fn], [fp, tp]])
+        M01 = confusion_matrix[0][1]
+        M11 = confusion_matrix[1][1]
+        M10 = confusion_matrix[1][0]
+        M00 = confusion_matrix[0][0]
+
+        FNR = M01 / (M01 + M11)
+        FPR = M10 / (M00 + M10)
+
+        [DCF, DCFnormal] = Bayes_risk(confusion_matrix, pi, Cfn, Cfp)
+
+        FNRlist = np.append(FNRlist, FNR)
+        FPRlist = np.append(FPRlist, FPR)
+        DCFnorm = np.append(DCFnorm, DCFnormal)
+    minDCF = min(DCFnorm)
+
+    return minDCF, FPRlist, FNRlist
```

