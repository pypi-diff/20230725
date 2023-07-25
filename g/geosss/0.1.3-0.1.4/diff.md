# Comparing `tmp/geosss-0.1.3.tar.gz` & `tmp/geosss-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosss-0.1.3.tar", max compression
+gzip compressed data, was "geosss-0.1.4.tar", max compression
```

## Comparing `geosss-0.1.3.tar` & `geosss-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1474 2023-07-24 16:27:27.579099 geosss-0.1.3/LICENSE
--rw-r--r--   0        0        0     4520 2023-07-24 17:29:37.459846 geosss-0.1.3/README.md
--rw-r--r--   0        0        0      874 2023-07-24 13:15:40.474358 geosss-0.1.3/geosss/__init__.py
--rw-r--r--   0        0        0     2008 2023-07-24 10:44:27.723589 geosss-0.1.3/geosss/demo_vis.py
--rw-r--r--   0        0        0     5526 2023-07-24 13:15:34.178370 geosss-0.1.3/geosss/distributions.py
--rw-r--r--   0        0        0    10315 2023-07-21 12:56:08.777564 geosss-0.1.3/geosss/mcmc.py
--rw-r--r--   0        0        0     5077 2023-07-20 16:23:21.588897 geosss-0.1.3/geosss/rand.py
--rw-r--r--   0        0        0     2970 2023-07-12 13:13:10.029358 geosss-0.1.3/geosss/sphere.py
--rw-r--r--   0        0        0     7405 2023-07-24 13:38:26.469573 geosss-0.1.3/geosss/testing.py
--rw-r--r--   0        0        0     5208 2023-07-21 12:35:35.101993 geosss-0.1.3/geosss/utils.py
--rw-r--r--   0        0        0     9267 2023-07-20 16:22:12.304818 geosss-0.1.3/geosss/vMF_diagnostics.py
--rw-r--r--   0        0        0      872 2023-07-24 17:29:49.055858 geosss-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 geosss-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1474 2023-07-24 16:27:27.579099 geosss-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4520 2023-07-24 17:29:37.459846 geosss-0.1.4/README.md
+-rw-r--r--   0        0        0      793 2023-07-25 18:15:32.875577 geosss-0.1.4/geosss/__init__.py
+-rw-r--r--   0        0        0     1981 2023-07-25 18:12:02.547408 geosss-0.1.4/geosss/demo_vis.py
+-rw-r--r--   0        0        0     5522 2023-07-25 18:15:09.487552 geosss-0.1.4/geosss/distributions.py
+-rw-r--r--   0        0        0    10284 2023-07-25 18:15:13.175555 geosss-0.1.4/geosss/mcmc.py
+-rw-r--r--   0        0        0     5091 2023-07-25 18:15:16.151557 geosss-0.1.4/geosss/rand.py
+-rw-r--r--   0        0        0     3000 2023-07-25 18:15:18.371559 geosss-0.1.4/geosss/sphere.py
+-rw-r--r--   0        0        0     7334 2023-07-25 18:16:16.463641 geosss-0.1.4/geosss/testing.py
+-rw-r--r--   0        0        0     5156 2023-07-25 18:15:26.103567 geosss-0.1.4/geosss/utils.py
+-rw-r--r--   0        0        0     9249 2023-07-25 18:15:30.843574 geosss-0.1.4/geosss/vMF_diagnostics.py
+-rw-r--r--   0        0        0      890 2023-07-25 18:24:36.544259 geosss-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5354 1970-01-01 00:00:00.000000 geosss-0.1.4/PKG-INFO
```

### Comparing `geosss-0.1.3/LICENSE` & `geosss-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geosss-0.1.3/README.md` & `geosss-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `geosss-0.1.3/geosss/demo_vis.py` & `geosss-0.1.4/geosss/demo_vis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,76 @@
-
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.colors import Normalize
 
 from geosss.distributions import Distribution
 
-METHODS = ('sss-reject', 'sss-shrink', 'rwmh', 'hmc')
-ALGOS = {'sss-reject': 'geoSSS (reject)', 'sss-shrink': 'geoSSS (shrink)',
-         'rwmh': 'RWMH', 'hmc': 'HMC'}
+METHODS = ("sss-reject", "sss-shrink", "rwmh", "hmc")
+ALGOS = {
+    "sss-reject": "geoSSS (reject)",
+    "sss-shrink": "geoSSS (shrink)",
+    "rwmh": "RWMH",
+    "hmc": "HMC",
+}
 
 
 def sphere_pdf(n_grid: int, pdf: Distribution):
-    """ spherical grid with pdf"""
+    """spherical grid with pdf"""
 
     # spherical grid
     u = np.linspace(0, np.pi, n_grid)
     v = np.linspace(0, 2 * np.pi, n_grid)
 
     u_grid, v_grid = np.meshgrid(u, v)
-    vertices = np.stack([np.cos(v_grid) * np.sin(u_grid),
-                        np.sin(v_grid) * np.sin(u_grid),
-                        np.cos(u_grid)],
-                        axis=2)
+    vertices = np.stack(
+        [
+            np.cos(v_grid) * np.sin(u_grid),
+            np.sin(v_grid) * np.sin(u_grid),
+            np.cos(u_grid),
+        ],
+        axis=2,
+    )
 
     # spherical to cartesian
     sph2cart = (
         np.outer(np.cos(v), np.sin(u)),
         np.outer(np.sin(v), np.sin(u)),
-        np.outer(np.ones_like(u), np.cos(u))
+        np.outer(np.ones_like(u), np.cos(u)),
     )
 
     # pdf values for the grid
     pdf_vals = np.array([np.exp(pdf.log_prob(val)) for val in vertices])
 
     return sph2cart, pdf_vals
 
 
 def compare_samplers_3d(
-        pdf: Distribution,
-        samples: dict,
-        n_grid: int = 100,
+    pdf: Distribution,
+    samples: dict,
+    n_grid: int = 100,
 ):
-
     for method in METHODS:
         msg = "visualization accepts only 3 dimension"
         assert samples[method].shape[1] == 3, msg
 
     sph2cart, pdf_vals = sphere_pdf(n_grid, pdf)
     pdfnorm = Normalize(vmin=pdf_vals.min(), vmax=pdf_vals.max())
 
-    fig, axes = plt.subplots(2, 2, figsize=(8, 8), subplot_kw={
-        "projection": "3d"}, sharex=True, sharey=True)
+    fig, axes = plt.subplots(
+        2, 2, figsize=(8, 8), subplot_kw={"projection": "3d"}, sharex=True, sharey=True
+    )
 
     for ax, method in zip(axes.flat, METHODS):
         ax.computed_zorder = False
-        ax.plot_surface(*sph2cart,
-                        facecolors=plt.cm.terrain_r(pdfnorm(pdf_vals)),
-                        alpha=1, zorder=1)
+        ax.plot_surface(
+            *sph2cart, facecolors=plt.cm.terrain_r(pdfnorm(pdf_vals)), alpha=1, zorder=1
+        )
 
         x = samples[method]
-        ax.scatter(*x.T, c='tab:red', s=1, alpha=0.4, zorder=2)
+        ax.scatter(*x.T, c="tab:red", s=1, alpha=0.4, zorder=2)
         ax.set_title(ALGOS[method], pad=-30)
-        ax.set_aspect('equal')
+        ax.set_aspect("equal")
         ax.view_init(-140, 150)
-        ax.axis('off')
+        ax.axis("off")
 
     fig.tight_layout()
     plt.show()
```

### Comparing `geosss-0.1.3/geosss/distributions.py` & `geosss-0.1.4/geosss/distributions.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,106 +7,99 @@
 from scipy.special import i0, ive, logsumexp
 
 from geosss import sphere
 from geosss.utils import counter
 
 
 class Distribution:
-
     def log_prob(self, x):
         pass
 
 
 class Uniform(Distribution):
-
     def log_prob(self, x):
-        return 0.
+        return 0.0
 
     def gradient(self, x):
         return np.zeros_like(x)
 
 
 @counter(["log_prob", "gradient"])
 class Bingham(Distribution):
     """Bingham distribution
 
-    p(x) \propto \exp(x^T A x) 
+    p(x) \propto \exp(x^T A x)
 
     where A is a symmetric matrix without loss of generality.
 
     We can use a spectral decomposition to write
     \[
     A = U\Lambda U^T
     \]
     where $\Lambda$ is diagonal matrix of eigenvalues, and the columns of $U$
-    are the eigenvectors of $A$. Moreover, $U$ is a column-orthogonal matrix: 
-    $U^T U = I$. 
+    are the eigenvectors of $A$. Moreover, $U$ is a column-orthogonal matrix:
+    $U^T U = I$.
 
     Variable transformation:
 
     x -> y = U^Tx, x = Uy
 
     The transformed distribution is
 
-    y \sim \exp(\sum_i \lambda_i y_i^2) = \prod_i \exp(\lambda_i y_i^2) 
+    y \sim \exp(\sum_i \lambda_i y_i^2) = \prod_i \exp(\lambda_i y_i^2)
 
     subject to $\|y\| = 1$
 
     \exp(x^T A x) : Bingham distribution
     \exp(x^T b) : von Mises - Fisher distribution
     \exp(x^T A x + x^T b): Fisher-Bingham distribution
     """
 
     def __init__(self, A):
-
         assert np.allclose(A, A.T)
 
         self.A = A
 
         # eigh returns eigenvalues/-vectors in ascending order
         v, U = np.linalg.eigh(A)
 
         # descending order
         self.v, self.U = v[::-1], U[:, ::-1]
 
     def log_prob(self, x):
         """
         Evaluate the log pdf of the Bingham distribution for a single point on
         the sphere (if np.ndim(x) == 1) or multiple points (rows of a rank-2
-        array). 
+        array).
         """
         assert x.ndim in (1, 2) and x.shape[-1] == self.d
 
         return np.sum((x @ self.A) * x, axis=-1)
 
     def gradient(self, x):
         return 2 * self.A @ x
 
     @property
     def d(self):
-        """Dimension of ambient space. 
-        """
+        """Dimension of ambient space."""
         return len(self.A)
 
     @property
     def mode(self):
-        """Point with maximum probability. 
-        """
+        """Point with maximum probability."""
         return self.U[:, 0]
 
     @property
     def max_log_prob(self):
         return self.v[0]
 
 
 @counter(["log_prob", "gradient"])
 class BinghamFisher(Bingham):
-
     def __init__(self, A, b):
-
         super().__init__(A)
         assert len(A) == len(b)
         self.b = b
 
     def log_prob(self, x):
         return super().log_prob(x) + x @ self.b
 
@@ -139,52 +132,51 @@
     def max_log_prob(self):
         return self.kappa
 
     @functools.cached_property
     def log_Z(self):
         d = self.d
         kappa = np.linalg.norm(self.mu)
-        log_Z = (d/2) * np.log(2 * np.pi) + np.log(ive(d/2 - 1, kappa)) - \
-            (d/2 - 2) * np.log(kappa)
+        log_Z = (
+            (d / 2) * np.log(2 * np.pi)
+            + np.log(ive(d / 2 - 1, kappa))
+            - (d / 2 - 2) * np.log(kappa)
+        )
         return log_Z
 
     def log_prob(self, x):
-        return x @ self.mu - np.log(2 * np.pi) \
-            - np.log(i0(np.linalg.norm(self.mu)))
+        return x @ self.mu - np.log(2 * np.pi) - np.log(i0(np.linalg.norm(self.mu)))
 
     def gradient(self, x):
         return self.mu
 
 
 @counter("log_prob")
 class MultivariateNormal(Distribution):
-
     def __init__(self, mu, C):
         self.mu = mu
         self.C = C
         self.invC = np.linalg.inv(C)
 
     def log_prob(self, x):
-        return -0.5 * np.sum((x-self.mu) * ((x-self.mu) @ self.invC), axis=-1)
+        return -0.5 * np.sum((x - self.mu) * ((x - self.mu) @ self.invC), axis=-1)
 
 
 @counter("log_prob")
 class ACG(MultivariateNormal):
-
     def __init__(self, C):
         super().__init__(np.zeros(len(C)), C)
 
     def log_prob(self, x):
         y = -2 * super().log_prob(x)
-        return - np.log(y) * len(self.C) / 2
+        return -np.log(y) * len(self.C) / 2
 
 
 @counter(["log_prob", "gradient"])
 class MixtureModel(Distribution):
-
     def __init__(self, components, weights=None):
         self.pdfs = components
         if weights is None:
             weights = np.ones(len(components))
         self.weights = np.array(weights)
         self.weights /= self.weights.sum()
 
@@ -208,15 +200,15 @@
     d : integer >= 2
         Dimension of ambient space
     vmax : float or None
         Optional maximum eigenvalue of the precision matrix.
     vmin : float or None
         Optional minimum eigenvalue of the precision matrix.
     eigensystem : bool
-        Flag specifying if Bingham distribution has diagonal precision matrix 
+        Flag specifying if Bingham distribution has diagonal precision matrix
         (i.e. we are working in the eigenvasis of A) or not. (Default value:
         False)
     """
     rng = np.random.default_rng(seed)
 
     A = rng.standard_normal((d, d))
     A = A.T @ A
```

### Comparing `geosss-0.1.3/geosss/mcmc.py` & `geosss-0.1.4/geosss/mcmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 
 from geosss import sphere
 
 
 def determine_burnin(n_samples, burnin):
     if isinstance(burnin, float):
-        assert 0 <= burnin <= 1.
+        assert 0 <= burnin <= 1.0
         return int(burnin * n_samples)
     else:
         assert burnin >= 0
         return int(burnin)
 
 
 class Sampler:
@@ -87,15 +87,15 @@
         is switched on in the initial phase of the simulation (burnin) and switched off
         after burn-in in order to ensure detailed balance.
     """
 
     def __init__(self, stepsize=1e-3, **kwargs):
         super().__init__(**kwargs)
         self.stepsize = float(stepsize)
-        assert self.stepsize > 0.
+        assert self.stepsize > 0.0
         self.reset(0)
 
     def reset(self, burnin):
         self._counter = 0
         self._burnin = int(burnin)
         self._burnin >= 0
 
@@ -106,15 +106,14 @@
         """
         if self._counter < self._burnin:
             self.stepsize *= 1.02 if accepted else 0.98
             self._counter += 1
 
 
 class MetropolisHastings(Sampler, AdaptiveStepsize):
-
     def __init__(self, distribution, initial_state, seed=None, stepsize=1e-1):
         """
         Parameters
         ----------
         distribution: instance of distributions.Distribution
             Target distribution implementing `log_prob`
 
@@ -165,33 +164,34 @@
         interpreted as percentage of the desired number of samples).
         """
         self.reset(determine_burnin(n_samples, burnin))
         return super().sample(n_samples, burnin)
 
 
 class IndependenceSampler(MetropolisHastings):
-
     def propose(self):
         x = self.rng.standard_normal(len(self.state))
         return sphere.radial_projection(x)
 
 
 def project(x, v):
     """
-    Project x into complement of v. 
+    Project x into complement of v.
     """
     return x - v * (v @ x)
 
 
 class SphericalHMC(MetropolisHastings):
     """
     Spherical Hamiltonian Monte Carlo.
     """
 
-    def __init__(self, distribution, initial_state, seed=None, stepsize=1e-3, n_steps=10):
+    def __init__(
+        self, distribution, initial_state, seed=None, stepsize=1e-3, n_steps=10
+    ):
         """
         Parameters
         ----------
         distribution: instance of distributions.Distribution
             Target distribution implementing `log_prob` and `gradient`
 
         initial_state: numpy ndarray
@@ -208,15 +208,15 @@
         """
         state = np.hstack([initial_state, np.zeros_like(initial_state)])
         super().__init__(distribution, state, seed, stepsize=stepsize)
         self.n_steps = int(n_steps)
 
     def sample_momenta(self):
         """
-        Sample momenta in spherical HMC. 
+        Sample momenta in spherical HMC.
         """
         x, v = np.reshape(self.state, (2, -1))
         v = project(self.rng.standard_normal(len(x)), x)
         self.state = np.hstack([x, v])
 
     def hamiltonian(self, state):
         """
@@ -236,15 +236,14 @@
         self.sample_momenta()
 
         x, v = np.reshape(np.copy(self.state), (2, -1))
 
         v += 0.5 * eps * project(gradient(x), x)
 
         for t in range(self.n_steps):
-
             norm = np.linalg.norm(v)
 
             y = np.copy(x)
             x = y * np.cos(eps * norm) + (v / norm) * np.sin(eps * norm)
             v = v * np.cos(eps * norm) - (y * norm) * np.sin(eps * norm)
 
             if t < self.n_steps - 1:
@@ -256,17 +255,15 @@
 
     def accept_reject(self, state):
         prob = self.hamiltonian(self.state) - self.hamiltonian(state)
         return np.log(self.rng.random()) < prob
 
     def sample(self, n_samples, burnin=0, return_momenta=False):
         samples = super().sample(n_samples, burnin)
-        positions, momenta = np.swapaxes(
-            np.reshape(samples, (n_samples, 2, -1)), 1, 0
-        )
+        positions, momenta = np.swapaxes(np.reshape(samples, (n_samples, 2, -1)), 1, 0)
         return (positions, momenta) if return_momenta else positions
 
 
 class RejectionSphericalSliceSampler(Sampler):
     """
     Geodesic Spherical Rejection Slice Sampler
     """
@@ -285,15 +282,14 @@
             Seed for the random number generator.
         """
 
         super().__init__(distribution, initial_state, seed)
         self.n_reject = 0
 
     def __next__(self):
-
         x = self.state
         p = self.target.log_prob
 
         # sample subsphere
         u = sphere.spherical_projection(self.rng.standard_normal(len(x)), x)
 
         threshold = p(x) + np.log(self.rng.random())
@@ -311,15 +307,14 @@
 
 class ShrinkageSphericalSliceSampler(RejectionSphericalSliceSampler):
     """
     Geodesic Spherical Shrinkage Slice Sampler
     """
 
     def __next__(self):
-
         x = self.state
         p = self.target.log_prob
 
         # sample subsphere
         u = sphere.spherical_projection(self.rng.standard_normal(len(x)), x)
 
         threshold = p(x) + np.log(self.rng.random())
@@ -329,10 +324,9 @@
 
         while True:
             theta = self.rng.uniform(*interval)
             y = np.cos(theta) * x + np.sin(theta) * u
             if p(y) > threshold:
                 self.state = y
                 return y
-            interval = (theta, interval[1]) if theta < 0 \
-                else (interval[0], theta)
+            interval = (theta, interval[1]) if theta < 0 else (interval[0], theta)
             self.n_reject += 1
```

### Comparing `geosss-0.1.3/geosss/rand.py` & `geosss-0.1.4/geosss/rand.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,121 +7,118 @@
 
 from geosss import distributions as dist
 from geosss import sphere
 
 
 def rotate_north(u):
     """
-    Find rotation of u onto north pole [0 ... 0 1]. 
+    Find rotation of u onto north pole [0 ... 0 1].
     """
     v = np.zeros_like(u)
     v[-1] = 1
 
     U, _, V = np.linalg.svd(np.multiply.outer(v, u))
 
     R = U @ V
 
-    if np.linalg.det(R) < 0.:
+    if np.linalg.det(R) < 0.0:
         U[:, -1] *= -1
         R = U @ V
 
     return R
 
 
 def sample_vMF(pdf, size=1):
     """
     Generates a random sample from the von Mises-Fisher distribution using the
-    algorithm proposed by Wood (1994). 
+    algorithm proposed by Wood (1994).
     """
     assert isinstance(pdf, dist.VonMisesFisher)
 
     if size > 1:
         return np.array([sample_vMF(pdf) for _ in range(int(size))])
 
     p = pdf.d - 1
     kappa = np.linalg.norm(pdf.mu)
 
-    if np.isclose(kappa, 0.):
+    if np.isclose(kappa, 0.0):
         return sphere.sample_sphere(p)
 
     u = pdf.mu / kappa
 
-    b0 = (-2 * kappa + (4 * kappa**2 + p**2)**0.5) / p
+    b0 = (-2 * kappa + (4 * kappa**2 + p**2) ** 0.5) / p
     x0 = (1 - b0) / (1 + b0)
     n = kappa * x0 + p * np.log(1 - x0**2)
 
     while True:
-
         Z = np.random.beta(0.5 * p, 0.5 * p)
         U = np.log(np.random.rand())
         W = (1 - (1 + b0) * Z) / (1 - (1 - b0) * Z)
 
         if (kappa * W + p * np.log(1 - x0 * W) - n) >= U:
             break
 
     # sample from d-2 sphere
-    v = sphere.sample_sphere(p-1)
-    x = np.append((1 - W**2)**0.5 * v, W)
+    v = sphere.sample_sphere(p - 1)
+    x = np.append((1 - W**2) ** 0.5 * v, W)
     R = rotate_north(u).T
 
     return R @ x
 
 
 def sample_bingham_2d(pdf, n_samples=1):
-    """Sample from 2D Bingham distribution. 
+    """Sample from 2D Bingham distribution.
 
     Sample from the 2D Bingham distribution by transforming it to a zero-
-    centered von Mises distribution. 
+    centered von Mises distribution.
     """
     if not (isinstance(pdf, dist.Bingham) and pdf.d == 2):
-        raise ValueError('expected 2D Bingham distribution')
+        raise ValueError("expected 2D Bingham distribution")
 
     u = np.random.choice([0, 1], size=int(n_samples))
     kappa = 0.5 * (pdf.v[0] - pdf.v[1])
-    phi = np.random.vonmises(0., kappa, int(n_samples))
+    phi = np.random.vonmises(0.0, kappa, int(n_samples))
 
     # von Mises is defined over [-pi, pi), we want phi to be defined over
     # [0, 2pi) therefore we need to shift it by pi
     # theta = 0.5 * np.squeeze(phi + (2 * u + 1) * np.pi)
     theta = 0.5 * np.squeeze(phi + 2 * u * np.pi)
 
     # Cartesian coordinates
     x = sphere.polar2cartesian(theta)
 
     return x @ pdf.U.T
 
 
 def sample_bingham_3d(pdf, n_samples=1):
-    """Sample from the 3D Bingham distribution by using a Gibbs sampler. 
-    """
+    """Sample from the 3D Bingham distribution by using a Gibbs sampler."""
     if not isinstance(pdf, dist.Bingham) or pdf.d != 3:
-        raise ValueError('3D Bingham expected')
+        raise ValueError("3D Bingham expected")
 
     v = pdf.v
 
     # initialization
-    x = np.random.uniform(-1., 1)
+    x = np.random.uniform(-1.0, 1)
     theta = np.arccos(x)
 
     samples = []
     while len(samples) < n_samples:
-
         # sample azimuthal angle phi
-        kappa = np.sin(theta)**2 * 0.5 * (v[0] - v[1])
+        kappa = np.sin(theta) ** 2 * 0.5 * (v[0] - v[1])
         u = np.random.choice([0, 1])
         # TODO: phi = 0.5 * (np.random.vonmises(0., kappa) + (2*u + 1) * np.pi)
-        phi = 0.5 * (np.random.vonmises(0., kappa) + 2*u * np.pi)
+        phi = 0.5 * (np.random.vonmises(0.0, kappa) + 2 * u * np.pi)
 
         # sample polar angle theta
-        kappa = v[2] + (v[1] - v[0]) * np.cos(phi)**2 - v[1]
-        C = 0. if kappa < 0 else kappa
+        kappa = v[2] + (v[1] - v[0]) * np.cos(phi) ** 2 - v[1]
+        C = 0.0 if kappa < 0 else kappa
 
         # rejection sampling of x=cos(theta)
         while True:
-            x = np.random.uniform(-1., 1.)
+            x = np.random.uniform(-1.0, 1.0)
             u = np.random.rand()
             if np.log(u) < kappa * x**2 - C:
                 theta = np.arccos(x)
                 break
 
         samples.append((phi, theta))
 
@@ -129,49 +126,51 @@
     x = sphere.spherical2cartesian(*np.transpose(samples))
 
     return x @ pdf.U.T
 
 
 def bfind(vals):
     """
-    `vals` are the eigenvalues of the precision matrix. 
+    `vals` are the eigenvalues of the precision matrix.
     """
-    def fb(b): return 1 - np.sum(1 / (b + 2 * vals))
-    if np.allclose(vals, 0.):
+
+    def fb(b):
+        return 1 - np.sum(1 / (b + 2 * vals))
+
+    if np.allclose(vals, 0.0):
         return len(vals)
     return brentq(fb, 1, len(vals))
 
 
 def sample_bingham(A, n_samples, n_iter=1000, return_efficiency=False):
     """
     Implementation of rejection sampling algorithm by Kent, Ganeiber and
-    Mardia. 
+    Mardia.
     """
     if A.ndim == 1:
         v = -A
     elif A.ndim == 2:
         v, U = np.linalg.eigh(-A)
 
     v -= np.min(v)
     b = bfind(v)
     log_M = -(len(A) - b) / 2 + (len(A) / 2) * np.log(len(A) / b)
 
     n = n_samples
     efficiency = []
     samples = []
     for _ in range(n_iter):
-
         # sample from angular central Gaussian (ACG) proposal
         x = np.random.randn(n, len(A)) / np.sqrt(1 + 2 * v / b)
         x /= np.linalg.norm(x, axis=-1)[:, None]
 
         # evaluate unnormalized ACG, Bingham, and bound
         u = np.sum(np.square(x) * v, axis=-1)
-        log_acg = - (len(A) / 2) * np.log(1 + 2 * u / b)
-        log_bing = - u
+        log_acg = -(len(A) / 2) * np.log(1 + 2 * u / b)
+        log_bing = -u
 
         # acceptance probability
         log_prob = log_bing - log_acg - log_M
 
         # accept / reject
         mask = np.log(np.random.rand(n)) < log_prob
         n -= np.sum(mask)
@@ -181,13 +180,13 @@
             break
 
     samples = np.concatenate(samples, 0)[:n_samples]
     if A.ndim == 2:
         samples = samples @ U.T
 
     if False:
-        print('mean efficiency:', np.mean(efficiency))
+        print("mean efficiency:", np.mean(efficiency))
 
     if return_efficiency:
         return samples, np.mean(efficiency)
 
     return samples
```

### Comparing `geosss-0.1.3/geosss/sphere.py` & `geosss-0.1.4/geosss/sphere.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,114 +4,126 @@
 import numpy as np
 
 # projections
 
 
 def radial_projection(x):
     """
-    Radial projection of (d+1)-dimensional point(s) to d-sphere. 
+    Radial projection of (d+1)-dimensional point(s) to d-sphere.
     """
     norm = np.linalg.norm(x, axis=-1) + 1e-100
     if x.ndim == 1:
         return x / norm
     else:
         return x / norm[:, None]
 
 
 def orthogonal_projection(x, y):
     """
-    Map point(s) `x` into orthogonal complement of point `y`. 
+    Map point(s) `x` into orthogonal complement of point `y`.
     """
     normal = radial_projection(y)
     return x - (x @ normal) * normal
 
 
 def spherical_projection(x, v):
     """
-    Map point(s) `x` into the great subsphere with pole `v`. 
+    Map point(s) `x` into the great subsphere with pole `v`.
     """
     return radial_projection(orthogonal_projection(x, v))
 
+
 # sampling
 
 
 def sample_sphere(d=2, size=None, seed=None):
     """
     Draw a random point from d-sphere by drawing a (d+1)-dimensional point from the
-    standard normal distribution and mapping it to d-sphere. 
+    standard normal distribution and mapping it to d-sphere.
     """
     rng = np.random.default_rng(seed)
-    x = rng.standard_normal(
-        d+1) if size is None else rng.standard_normal((size, d+1))
+    x = (
+        rng.standard_normal(d + 1)
+        if size is None
+        else rng.standard_normal((size, d + 1))
+    )
     return radial_projection(x)
 
 
 def sample_subsphere(v, seed=None):
     """
     Sample uniformly from the great subsphere with pole `v`.
     """
     rng = np.random.default_rng(seed)
     return spherical_projection(rng.standard_normal(len(v)), v)
 
+
 # distances
 
 
 def distance(x, y):
     """
-    Great circle distance (assuming x, y are on the sphere). 
+    Great circle distance (assuming x, y are on the sphere).
     """
     return np.arccos(np.clip(np.sum(x * y, axis=-1), -1, 1))
 
 
 # transformation between Cartesian and polar coordinates
 
+
 def cartesian2polar(x):
     """Map points on the unit sphere to polar coordinates."""
-    return np.mod(np.arctan2(x[:, 1], x[:, 0]), 2*np.pi)
+    return np.mod(np.arctan2(x[:, 1], x[:, 0]), 2 * np.pi)
 
 
 def polar2cartesian(theta):
     return np.transpose([np.cos(theta), np.sin(theta)])
 
 
 def spherical2cartesian(phi, theta):
-    return np.transpose([np.cos(phi) * np.sin(theta),
-                         np.sin(phi) * np.sin(theta),
-                         np.cos(theta)])
+    return np.transpose(
+        [np.cos(phi) * np.sin(theta), np.sin(phi) * np.sin(theta), np.cos(theta)]
+    )
 
 
 def cartesian2spherical(x):
     return cartesian2polar(x), np.mod(np.arccos(x[:, 2]), np.pi)
 
 
 def sample_marginal(d, size=None, seed=None):
     rng = np.random.default_rng(seed)
-    s = rng.beta(0.5, 0.5 * (d-1), size=size)
+    s = rng.beta(0.5, 0.5 * (d - 1), size=size)
     t = np.sqrt(s) * rng.choice([-1, 1], size=size)
     return t
 
 
 def wrap(x, u, v):
-    """See Mardia and Jupp for 'wrapping approach'. """
+    """See Mardia and Jupp for 'wrapping approach'."""
     theta = np.linalg.norm(x)
     return np.sin(theta) * u + np.cos(theta) * v
 
 
 def slerp(u, v):
     theta = np.arccos(u @ v)
 
     def interpolation(phi, u=u, v=v, theta=theta):
-        return (np.sin(phi) * v + np.sin(theta-phi) * u) / np.sin(theta)
+        return (np.sin(phi) * v + np.sin(theta - phi) * u) / np.sin(theta)
+
     return interpolation
 
 
 def givens(u, v, x):
     """
     Returns function that rotates `x` in the plane spanned by `u`, `v` by an
-    angle that will be the argument of the function. 
+    angle that will be the argument of the function.
     """
+
     def rotate(theta, u=u, v=v, x=x):
         ux = u @ x
         vx = v @ x
-        return x + (np.cos(theta) - 1) * (ux * u + vx * v) \
+        return (
+            x
+            + (np.cos(theta) - 1) * (ux * u + vx * v)
             + np.sin(theta) * (ux * v - vx * u)
+        )
+
     return rotate
```

### Comparing `geosss-0.1.3/geosss/testing.py` & `geosss-0.1.4/geosss/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # preliminary implementation for variants of slice samplers
 
-import matplotlib.pyplot as plt
 import numpy as np
-from csb.statistics import autocorrelation
 
 from . import sphere
 
 # some nice colors
-colors = [(.85, .3, .1), (.15, .35, .6),
-          (.95, .7, 0.1), (.0, .0, .0), (.8, .8, .8)]
+colors = [
+    (0.85, 0.3, 0.1),
+    (0.15, 0.35, 0.6),
+    (0.95, 0.7, 0.1),
+    (0.0, 0.0, 0.0),
+    (0.8, 0.8, 0.8),
+]
 
 
 def sample_slice(log_prob, current, bounds, return_n_reject=False):
     """
-    Bracketing procedure as presented in the paper. 
+    Bracketing procedure as presented in the paper.
     """
     threshold = log_prob(current) + np.log(np.random.rand())
     L, R = bounds
     x = np.random.uniform(0, 2 * np.pi)
     L, R = x - 2 * np.pi, x
     n_reject = 0
 
@@ -33,15 +36,15 @@
         else:
             R = x
         n_reject += 1
 
 
 def sample_slice2(log_prob, current, bounds):
     """
-    Alternative version in which the brackets are first shifted. 
+    Alternative version in which the brackets are first shifted.
     """
     threshold = log_prob(current) + np.log(np.random.rand())
     x = np.random.uniform(*bounds)
     L, R = x + bounds[0], x + bounds[1]
 
     while True:
         if log_prob(x) > threshold:
@@ -49,229 +52,224 @@
         elif x < current:
             L = x
         else:
             R = x
         x = np.random.uniform(L, R)
 
 
-def metropolis_hastings(pdf, n_samples, stepsize=0.5, adapt_stepsize=False,
-                        reproject=True):
+def metropolis_hastings(
+    pdf, n_samples, stepsize=0.5, adapt_stepsize=False, reproject=True
+):
     """
-    Sample hyperspherical distribution with Metropolis Hastings. 
+    Sample hyperspherical distribution with Metropolis Hastings.
     """
     samples = []
-    x = sphere.sample_sphere(pdf.d-1)
+    x = sphere.sample_sphere(pdf.d - 1)
     n_acc = 0
 
     while len(samples) < n_samples:
-
         # propose
-        r = np.sqrt(np.random.gamma(0.5 * len(x)) / 0.5) if reproject else 1.
+        r = np.sqrt(np.random.gamma(0.5 * len(x)) / 0.5) if reproject else 1.0
         y = sphere.radial_projection(r * x + stepsize * np.random.randn(pdf.d))
 
         # accept / reject
         accept = np.log(np.random.rand()) < pdf.log_prob(y) - pdf.log_prob(x)
         x = y if accept else x
 
         # adapt stepsize
         if adapt_stepsize:
             stepsize *= 1.02 if accept else 0.98
 
         samples.append(np.copy(x))
         n_acc += int(accept)
 
-    print(f'stepsize: {stepsize}, acceptance rate: {(n_acc/n_samples):.1%}')
+    print(f"stepsize: {stepsize}, acceptance rate: {(n_acc/n_samples):.1%}")
 
     return np.array(samples)
 
 
 def slice_sampling(pdf, n_samples=1e3):
-    """ 
-    Slice sampling on the sphere using first bracketing procedure. 
+    """
+    Slice sampling on the sphere using first bracketing procedure.
     """
     bounds = (-np.pi, np.pi)
 
     # initialization
-    v = sphere.sample_sphere(pdf.d-1)
+    v = sphere.sample_sphere(pdf.d - 1)
     samples = [v]
     n_reject = []
 
     while len(samples) < n_samples:
-
         # draw uniformly from subsphere
         u = sphere.sample_subsphere(v)
 
         # define probability on slice
-        def log_prob(theta, pdf=pdf, v=v, u=u): return \
-            pdf.log_prob(np.cos(theta) * v + np.sin(theta) * u)
+        def log_prob(theta, pdf=pdf, v=v, u=u):
+            return pdf.log_prob(np.cos(theta) * v + np.sin(theta) * u)
 
         # slice sampling using first bracketing procedure starting at current
         # sample (corresponding to theta=0)
-        theta, n = sample_slice(log_prob, 0., bounds, return_n_reject=True)
+        theta, n = sample_slice(log_prob, 0.0, bounds, return_n_reject=True)
 
         v = np.cos(theta) * v + np.sin(theta) * u
 
         samples.append(v)
         n_reject.append(n)
 
-    print(f'average number of rejections: {np.mean(n_reject)}')
+    print(f"average number of rejections: {np.mean(n_reject)}")
 
     return np.array(samples)
 
 
 def slice_sampling2(pdf, n_samples=1e3):
-    """ 
-    Slice sampling on the sphere using second bracketing procedure. 
+    """
+    Slice sampling on the sphere using second bracketing procedure.
     """
     bounds = (-np.pi, np.pi)
 
     # initialization
-    v = sphere.sample_sphere(pdf.d-1)
+    v = sphere.sample_sphere(pdf.d - 1)
     samples = [v]
     n_reject = []
 
     while len(samples) < n_samples:
-
         # draw uniformly from subsphere
         u = sphere.sample_subsphere(v)
 
         # define probability on slice
-        def log_prob(theta, pdf=pdf, v=v, u=u): return \
-            pdf.log_prob(np.cos(theta) * v + np.sin(theta) * u)
+        def log_prob(theta, pdf=pdf, v=v, u=u):
+            return pdf.log_prob(np.cos(theta) * v + np.sin(theta) * u)
 
         # slice sampling using second bracketing procedure starting at current
         # sample (corresponding to theta=0)
-        theta, n = sample_slice2(log_prob, 0., bounds, return_n_reject=True)
+        theta, n = sample_slice2(log_prob, 0.0, bounds, return_n_reject=True)
 
         v = np.cos(theta) * v + np.sin(theta) * u
 
         samples.append(v)
         n_reject.append(n)
 
-    print(f'average number of rejections: {np.mean(n_reject)}')
+    print(f"average number of rejections: {np.mean(n_reject)}")
 
     return np.array(samples)
 
 
 def slice_sampling3(pdf, n_samples=1e3):
-    """ 
-    Slice sampling on the sphere using slerp and bracketing. 
+    """
+    Slice sampling on the sphere using slerp and bracketing.
     """
     # initialization
-    v = sphere.sample_sphere(pdf.d-1)
+    v = sphere.sample_sphere(pdf.d - 1)
 
     samples = [v]
     n_reject = []
 
     while len(samples) < n_samples:
-
         # draw uniformly from sphere
-        u = sphere.sample_sphere(pdf.d-1)
+        u = sphere.sample_sphere(pdf.d - 1)
 
         # slerp
         slerp = sphere.slerp(u, v)
         theta = np.arccos(u @ v)  # - 0.5 * np.pi
 
         bounds = (theta - np.pi, theta + np.pi)
 
         # define probability on slice
-        def log_prob(theta, pdf=pdf, slerp=slerp): return \
-            pdf.log_prob(slerp(theta))
+        def log_prob(theta, pdf=pdf, slerp=slerp):
+            return pdf.log_prob(slerp(theta))
 
         # slice sampling using first bracketing procedure starting at current
         # sample (corresponding to theta=0)
         theta, n = sample_slice(log_prob, theta, bounds, return_n_reject=True)
 
         v = slerp(theta)
 
         samples.append(v)
         n_reject.append(n)
 
-    print(f'average number of rejections: {np.mean(n_reject)}')
+    print(f"average number of rejections: {np.mean(n_reject)}")
 
     return np.array(samples)
 
 
 def slice_sampling4(pdf, n_samples=1e3):
-    """ 
-    Slice sampling on the sphere using random Givens rotations and bracketing. 
+    """
+    Slice sampling on the sphere using random Givens rotations and bracketing.
     """
     bounds = (-np.pi, np.pi)
 
     # initialization
-    x = sphere.sample_sphere(pdf.d-1)
+    x = sphere.sample_sphere(pdf.d - 1)
 
     samples = [x]
     n_reject = []
 
     while len(samples) < n_samples:
-
         # draw uniformly from sphere
-        u = sphere.sample_sphere(pdf.d-1)
-        v = sphere.sample_sphere(pdf.d-1)  # generates a small circle?
+        u = sphere.sample_sphere(pdf.d - 1)
+        v = sphere.sample_sphere(pdf.d - 1)  # generates a small circle?
 
         # how to construct a great circle?
         v = x  # also generates a small circle
         # unless
         u = sphere.spherical_projection(u, x)
 
         # Givens rotation
         givens = sphere.givens(u, v, x)
 
         # define probability on slice
-        def log_prob(theta, pdf=pdf, givens=givens): return \
-            pdf.log_prob(givens(theta))
+        def log_prob(theta, pdf=pdf, givens=givens):
+            return pdf.log_prob(givens(theta))
 
-        assert np.isclose(log_prob(0.), pdf.log_prob(x))
+        assert np.isclose(log_prob(0.0), pdf.log_prob(x))
 
         # slice sampling using first bracketing procedure starting at current
         # sample (corresponding to theta=0)
-        theta, n = sample_slice(log_prob, 0., bounds, return_n_reject=True)
+        theta, n = sample_slice(log_prob, 0.0, bounds, return_n_reject=True)
 
         x = givens(theta)
 
         samples.append(x)
         n_reject.append(n)
 
-    print(f'average number of rejections: {np.mean(n_reject)}')
+    print(f"average number of rejections: {np.mean(n_reject)}")
 
     return np.array(samples)
 
 
 def spherical_rejection_sampling(pdf, n_samples=1e3):
-    """ 
-    Use rejection sampling to sample from slice. 
+    """
+    Use rejection sampling to sample from slice.
     """
     bounds = (-np.pi, np.pi)
     bounds = (0, 2 * np.pi)
 
     # initialization
-    v = sphere.sample_sphere(pdf.d-1)
+    v = sphere.sample_sphere(pdf.d - 1)
     samples = [v]
 
     n_reject = []
     while len(samples) < n_samples:
-
         # draw uniformly from subsphere
         u = sphere.sample_subsphere(v)
 
         # define probability on slice
-        def log_prob(theta, pdf=pdf, v=v, u=u): return \
-            pdf.log_prob(np.cos(theta) * v + np.sin(theta) * u)
+        def log_prob(theta, pdf=pdf, v=v, u=u):
+            return pdf.log_prob(np.cos(theta) * v + np.sin(theta) * u)
 
         # rejection sampling where current sample defines threshold
-        threshold = log_prob(0.) + np.log(np.random.rand())
+        threshold = log_prob(0.0) + np.log(np.random.rand())
         n = 0
         while True:
             theta = np.random.uniform(*bounds)
             if log_prob(theta) > threshold:
                 n_reject.append(n)
                 break
             n += 1
 
         v = np.cos(theta) * v + np.sin(theta) * u
 
         samples.append(v)
 
-    print(f'average number of rejections: {np.mean(n_reject)}')
+    print(f"average number of rejections: {np.mean(n_reject)}")
 
     return np.array(samples)
```

### Comparing `geosss-0.1.3/geosss/utils.py` & `geosss-0.1.4/geosss/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,98 +1,109 @@
 import contextlib
 import time
 from functools import wraps
 
 import numpy as np
 from csb.numeric import log
 
-from geosss.mcmc import (MetropolisHastings, RejectionSphericalSliceSampler,
-                         ShrinkageSphericalSliceSampler, SphericalHMC)
+from geosss.mcmc import (
+    MetropolisHastings,
+    RejectionSphericalSliceSampler,
+    ShrinkageSphericalSliceSampler,
+    SphericalHMC,
+)
 
 # some nice colors
-colors = [(.85, .3, .1), (.15, .35, .6),
-          (.95, .7, 0.1), (.0, .0, .0), (.8, .8, .8)]
+colors = [
+    (0.85, 0.3, 0.1),
+    (0.15, 0.35, 0.6),
+    (0.95, 0.7, 0.1),
+    (0.0, 0.0, 0.0),
+    (0.8, 0.8, 0.8),
+]
 
 
 def format_time(t):
-
-    units = [(1., 's'), (1e-3, 'ms'), (1e-6, 'us'), (1e-9, 'ns')]
+    units = [(1.0, "s"), (1e-3, "ms"), (1e-6, "us"), (1e-9, "ns")]
     for scale, unit in units:
         if t > scale or t == 0:
             break
 
-    return '{0:.1f} {1}'.format(t/scale, unit)
+    return "{0:.1f} {1}".format(t / scale, unit)
 
 
 @contextlib.contextmanager
 def take_time(desc, mute=False):
     t0 = time.process_time()
     yield
     dt = time.process_time() - t0
     if not mute:
-        print('{0} took {1}'.format(desc, format_time(dt)))
+        print("{0} took {1}".format(desc, format_time(dt)))
 
 
 def relative_entropy(p, q):
-    """Kullback-Leibler divergence (aka as relative entropy). """
+    """Kullback-Leibler divergence (aka as relative entropy)."""
     return p @ (log(p) - log(q))
 
 
 def acf(x, n_max=None):
     """Autocorrelation.
 
     Parameters
     ----------
     x : 1d array
     n_max : maximum lag (if None then len(x) // 2)
 
     Returns
     -------
-    Array storing the estimated autocorrelation. 
+    Array storing the estimated autocorrelation.
     """
     n_max = n_max or len(x) // 2
     x = x - np.mean(x)
-    ac = [np.mean(x[i:] * x[:len(x) - i]) for i in range(n_max)]
+    ac = [np.mean(x[i:] * x[: len(x) - i]) for i in range(n_max)]
     return np.array(ac) / ac[0]
 
 
 def acf_fft(x):
     """Compute autocorrelation function using the convolution theorem."""
     X = np.fft.rfft((x - x.mean()) / x.std())
-    return np.real(np.fft.irfft(X.conj() * X))[:len(x)//2] / len(x)
+    return np.real(np.fft.irfft(X.conj() * X))[: len(x) // 2] / len(x)
 
 
 def IAT(x, n=None):
     """Computes the integrated autocorrelation time for given values by the heuristics
     described in Gelman et al "Bayesian Data Analysis", Chapter 11.5
     """
     ac = acf_fft(x)
     if n:
         ac = ac[:n]
-    sums = ac[2:-1].reshape(-1, 2).sum(1) if (len(ac) % 2 != 0) \
+    sums = (
+        ac[2:-1].reshape(-1, 2).sum(1)
+        if (len(ac) % 2 != 0)
         else ac[2:].reshape(-1, 2).sum(1)
+    )
     T = np.nonzero(sums < 0)[0][0]
-    L = (1 + 2 * T) if np.sum(sums < 0) else len(ac)-1
-    return 1.0 + np.max([2 * np.sum(ac[1:L+1]), 0.0])
+    L = (1 + 2 * T) if np.sum(sums < 0) else len(ac) - 1
+    return 1.0 + np.max([2 * np.sum(ac[1 : L + 1]), 0.0])
 
 
 def n_eff(x, n=None):
-    """Computes effective sample size n_eff for given values
-    """
+    """Computes effective sample size n_eff for given values"""
     return len(x) / IAT(x, n)
 
 
 def count_calls(func):
     """
-    decorator that counts how many times a method/function was called. If needed 
-    could be called directly only on a function with @count_calls 
+    decorator that counts how many times a method/function was called. If needed
+    could be called directly only on a function with @count_calls
     """
+
     @wraps(func)
     def wrapper(*args, **kwargs):
-        """ wrapper inside the `count_calls`"""
+        """wrapper inside the `count_calls`"""
         # updates the counter everytime func is called
         wrapper.num_calls += 1
         return func(*args, **kwargs)
 
     # counter starts
     wrapper.num_calls = 0
 
@@ -103,16 +114,16 @@
     wrapper.reset_counters = reset_counters
 
     return wrapper
 
 
 def counter(method_names):
     """
-    A decorator that counts how many times a method was called. It calls the `count_calls` function to 
-    wrap around a class. So it should be used only on a class. Example: @counter("some_method") or 
+    A decorator that counts how many times a method was called. It calls the `count_calls` function to
+    wrap around a class. So it should be used only on a class. Example: @counter("some_method") or
     @counter(["some_method", "another_method"])
 
     Args:
         method_names (str or list): the name(s) of the method(s) to decorate.
 
     Returns:
         A class decorator.
@@ -121,64 +132,58 @@
     if isinstance(method_names, str):
         method_names = [method_names]
 
     # `class_decorator` calls `count_calls` decorator
     def class_decorator(cls):
         for method_name in method_names:
             if hasattr(cls, method_name):
-                setattr(cls, method_name, count_calls(
-                    getattr(cls, method_name)))
+                setattr(cls, method_name, count_calls(getattr(cls, method_name)))
         return cls
 
     return class_decorator
 
 
 class SamplerLauncher:
-    """Just an interface for launching all the samplers
-    """
+    """Just an interface for launching all the samplers"""
 
     def __init__(self, pdf, initial, n_samples, burnin=0.2, seed=None):
         self.pdf = pdf
         self.initial = initial
         self.n_samples = n_samples
         self.burnin = burnin
         self.seed = seed
 
     def run_sss_reject(self):
-        sampler = RejectionSphericalSliceSampler(
-            self.pdf, self.initial, self.seed)
+        sampler = RejectionSphericalSliceSampler(self.pdf, self.initial, self.seed)
         self.rsss = sampler
 
         return sampler.sample(self.n_samples, burnin=self.burnin)
 
     def run_sss_shrink(self):
-        sampler = ShrinkageSphericalSliceSampler(
-            self.pdf, self.initial, self.seed)
+        sampler = ShrinkageSphericalSliceSampler(self.pdf, self.initial, self.seed)
         self.ssss = sampler
 
         return sampler.sample(self.n_samples, burnin=self.burnin)
 
     def run_rwmh(self):
-        sampler = MetropolisHastings(
-            self.pdf, self.initial, self.seed, stepsize=1e-1)
+        sampler = MetropolisHastings(self.pdf, self.initial, self.seed, stepsize=1e-1)
         self.rwmh = sampler
 
         return sampler.sample(self.n_samples, burnin=self.burnin)
 
     def run_hmc(self):
-        sampler = SphericalHMC(self.pdf, self.initial,
-                               self.seed, stepsize=1e-1)
+        sampler = SphericalHMC(self.pdf, self.initial, self.seed, stepsize=1e-1)
         self.hmc = sampler
 
         return sampler.sample(self.n_samples, burnin=self.burnin)
 
     def run(self, method):
-        if method == 'sss-reject':
+        if method == "sss-reject":
             return self.run_sss_reject()
-        elif method == 'sss-shrink':
+        elif method == "sss-shrink":
             return self.run_sss_shrink()
-        elif method == 'rwmh':
+        elif method == "rwmh":
             return self.run_rwmh()
-        elif method == 'hmc':
+        elif method == "hmc":
             return self.run_hmc()
         else:
-            raise ValueError(f'method {method} not known')
+            raise ValueError(f"method {method} not known")
```

### Comparing `geosss-0.1.3/geosss/vMF_diagnostics.py` & `geosss-0.1.4/geosss/vMF_diagnostics.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,86 +7,94 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from csb.io import dump, load
 
 from geosss.sphere import distance
 from geosss.utils import acf
 
-METHODS = ['sss-reject', 'sss-shrink', 'rwmh', 'hmc']
-ALGOS = {'sss-reject': 'geoSSS (reject)',
-         'sss-shrink': 'geoSSS (shrink)',
-         'rwmh': 'RWMH',
-         'hmc': 'HMC'}
+METHODS = ["sss-reject", "sss-shrink", "rwmh", "hmc"]
+ALGOS = {
+    "sss-reject": "geoSSS (reject)",
+    "sss-shrink": "geoSSS (shrink)",
+    "rwmh": "RWMH",
+    "hmc": "HMC",
+}
 
 plt.rc("font", size=16)
 
 
 def hist_plot(samples, ndim, path, filename, fs=16, save_res=False):
-    """ 
-    histogram of samples. 
+    """
+    histogram of samples.
     """
     bins = 100
     plt.rc("font", size=fs)
 
     # shows a standard histogram per dimension
     if ndim == 3:
         figsize = (10, 10)
     else:
         figsize = (10, 15)
-    fig, rows = plt.subplots(ndim, len(METHODS), figsize=figsize,
-                             sharex=True)
+    fig, rows = plt.subplots(ndim, len(METHODS), figsize=figsize, sharex=True)
 
     for i, axes in enumerate(rows):
-
         # reference samples
-        wood_vals = samples['wood'][:, i]
+        wood_vals = samples["wood"][:, i]
         ref = list(np.histogram(wood_vals, bins=bins, density=True))
         ref[1] = 0.5 * (ref[1][1:] + ref[1][:-1])
 
         # show histogram
         for ax, method in zip(axes, METHODS):
             marginals = samples[method][:, i]
 
-            bins = ax.hist(marginals, bins=bins, density=True, alpha=0.3,
-                           color='k', histtype='stepfilled')[1]
-            ax.plot(*ref[::-1], color='r', lw=1, ls='--')
-            ax.set_xlabel(fr'$e_{i}^Tx_n$', fontsize=fs)
+            bins = ax.hist(
+                marginals,
+                bins=bins,
+                density=True,
+                alpha=0.3,
+                color="k",
+                histtype="stepfilled",
+            )[1]
+            ax.plot(*ref[::-1], color="r", lw=1, ls="--")
+            ax.set_xlabel(rf"$e_{i}^Tx_n$", fontsize=fs)
 
     for ax, method in zip(rows[0], METHODS):
         ax.set_title(ALGOS[method], fontsize=fs)
     fig.tight_layout()
 
     if save_res:
         print(f"Saving sampler marginals plot..")
         fig.savefig(f"{path}/{filename}_hist.pdf", transparent=True)
 
     plt.close(fig)
 
 
 def trace_plots(samples, ndim, path, filename, fs=16, save_res=False):
-    """ 
+    """
     trace plots per dimension
     """
 
     os.makedirs(f"{path}/trace_plots", exist_ok=True)
 
     for d in range(ndim):
-        fig, axes = plt.subplots(1, len(METHODS), figsize=(
-            12, 5), sharex=True, sharey=True)
+        fig, axes = plt.subplots(
+            1, len(METHODS), figsize=(12, 5), sharex=True, sharey=True
+        )
 
         for ax, method in zip(axes, METHODS):
             ax.set_title(ALGOS[method], fontsize=fs)
-            ax.plot(samples[method][:, d], alpha=0.5, color='k', lw=1)
-            ax.set_xlabel(r'MCMC step $n$', fontsize=fs)
-        axes[0].set_ylabel(r'$u_{d}^Tx_n$', fontsize=fs)
-        fig.suptitle(fr"Trace plot $d_{{{d+1}}}$")
+            ax.plot(samples[method][:, d], alpha=0.5, color="k", lw=1)
+            ax.set_xlabel(r"MCMC step $n$", fontsize=fs)
+        axes[0].set_ylabel(r"$u_{d}^Tx_n$", fontsize=fs)
+        fig.suptitle(rf"Trace plot $d_{{{d+1}}}$")
         if save_res:
             print(f"saving trace plot for dimension {d+1}..")
             fig.savefig(
-                f"{path}/trace_plots/{filename}_trace_d{d+1}.pdf", transparent=True)
+                f"{path}/trace_plots/{filename}_trace_d{d+1}.pdf", transparent=True
+            )
 
         plt.close(fig)
 
 
 def acf_plots(samples, ndim, path, filename, lag=1000, fs=16, save_res=False):
     """
     Plots acf for every dimension in a multidimensional target
@@ -97,29 +105,28 @@
     for d in range(ndim):
         fig, ax = plt.subplots(1, 1, figsize=(6, 5))
 
         for method in METHODS:
             ac = acf(samples[method][:, d], lag)
             ax.plot(ac, alpha=0.7, lw=3, label=ALGOS[method])
             ax.legend(fontsize=fs)
-            ax.axhline(0., ls='--', color='k', alpha=0.7)
-            ax.set_xlabel(r'Lag', fontsize=fs)
-            ax.set_ylabel('ACF', fontsize=fs)
-            ax.set_title(fr"$d_{{{d+1}}}$")
+            ax.axhline(0.0, ls="--", color="k", alpha=0.7)
+            ax.set_xlabel(r"Lag", fontsize=fs)
+            ax.set_ylabel("ACF", fontsize=fs)
+            ax.set_title(rf"$d_{{{d+1}}}$")
         if save_res:
             print(f"saving acf plots for dim {d+1}..")
-            fig.savefig(
-                f"{path}/acf_plots/{filename}_acf_d{d+1}.pdf", transparent=True)
+            fig.savefig(f"{path}/acf_plots/{filename}_acf_d{d+1}.pdf", transparent=True)
 
         plt.close(fig)
 
 
 def acf_entropy_plot(samples, pdf, path, filename, lag=1000, fs=16, save_res=False):
-    """ 
-    ACF entropy plot 
+    """
+    ACF entropy plot
     """
 
     # population of modes
     modes = np.array([p.mu for p in pdf.pdfs])
 
     # kl-divergence and entropy
     KL = []
@@ -136,36 +143,36 @@
 
     fig, axes = plt.subplots(1, 2, figsize=(10, 4))
     ax = axes[0]
     for method in METHODS:
         ac = acf(samples[method][:, 0], lag)
         ax.plot(ac, alpha=0.7, lw=3, label=ALGOS[method])
     ax.legend(fontsize=fs)
-    ax.axhline(0., ls='--', color='k', alpha=0.7)
-    ax.set_xlabel(r'Lag', fontsize=fs)
-    ax.set_ylabel('ACF', fontsize=fs)
+    ax.axhline(0.0, ls="--", color="k", alpha=0.7)
+    ax.set_xlabel(r"Lag", fontsize=fs)
+    ax.set_ylabel("ACF", fontsize=fs)
 
     # hopping frequency as bar plot
     ax = axes[1]
     ax.set_ylabel("Entropy")
-    ax.bar(list(map(ALGOS.get, METHODS)), H, color='k', alpha=0.3)
-    ax.axhline(np.log(len(pdf.pdfs)), ls='--', color='r', label='max entropy')
+    ax.bar(list(map(ALGOS.get, METHODS)), H, color="k", alpha=0.3)
+    ax.axhline(np.log(len(pdf.pdfs)), ls="--", color="r", label="max entropy")
     plt.xticks(rotation=30)
     fig.tight_layout()
 
     if save_res:
         print(f"Saving ACF-Entropy plot..")
         fig.savefig(f"{path}/{filename}_acf_entropy.pdf", transparent=True)
 
     plt.close(fig)
 
 
 def entropy_kld(samples, pdf, path, filename, save_res=False):
-    """ 
-    Plots entropy and KL divergence plot between 
+    """
+    Plots entropy and KL divergence plot between
     target and sampled distribution
     """
 
     # population of modes
     modes = np.array([p.mu for p in pdf.pdfs])
     KL = []
     H = []
@@ -178,102 +185,101 @@
         p[i] /= p.sum()
         KL.append(p @ np.log(p / pdf.weights))
         H.append(-(p @ np.log(p)))
 
     fig, axes = plt.subplots(1, 1, figsize=(6, 4))
     ax = axes
     ax.set_ylabel("KL divergence")
-    ax.bar(list(map(ALGOS.get, METHODS)), KL, color='k', alpha=0.3)
+    ax.bar(list(map(ALGOS.get, METHODS)), KL, color="k", alpha=0.3)
     plt.xticks(rotation=30)
     fig.tight_layout()
     if save_res:
         print(f"Saving KL divergence plot..")
-        fig.savefig(f"{path}/{filename}_kl.pdf",
-                    bbox_inches='tight', transparent=True)
+        fig.savefig(f"{path}/{filename}_kl.pdf", bbox_inches="tight", transparent=True)
 
     fig, axes = plt.subplots(1, 1, figsize=(6, 4))
     ax = axes
     ax.set_ylabel("Entropy")
-    ax.bar(list(map(ALGOS.get, METHODS)), H, color='k', alpha=0.3)
+    ax.bar(list(map(ALGOS.get, METHODS)), H, color="k", alpha=0.3)
     plt.xticks(rotation=30)
     fig.tight_layout()
     if save_res:
         print(f"Saving entropy plot..")
-        fig.savefig(f"{path}/{filename}_entropy.pdf",
-                    bbox_inches='tight', transparent=True)
+        fig.savefig(
+            f"{path}/{filename}_entropy.pdf", bbox_inches="tight", transparent=True
+        )
 
     plt.close(fig)
 
 
 def dist_plot(samples, pdf, kappa, path, filename, fs=16, save_res=False):
-    """ 
+    """
     plotting Geodesic distance
     """
 
     modes = np.array([p.mu for p in pdf.pdfs])
-    d_modes = np.concatenate(
-        [distance(modes/kappa, mode/kappa) for mode in modes])
+    d_modes = np.concatenate([distance(modes / kappa, mode / kappa) for mode in modes])
     d_modes = np.unique(np.round(d_modes, 5))
-    fig, axes = plt.subplots(1, len(METHODS), figsize=(len(METHODS) * 3, 3),
-                             sharex=True, sharey=True)
+    fig, axes = plt.subplots(
+        1, len(METHODS), figsize=(len(METHODS) * 3, 3), sharex=True, sharey=True
+    )
     bins = 100
     for ax, method in zip(axes, METHODS):
         ax.set_title(ALGOS[method], fontsize=fs)
 
         # distance between successive samples
         x = samples[method]
         d = distance(x[:-1], x[1:])
-        print('average great circle distance of successive samples: '
-              f'{np.mean(d):.2f} ({method})')
+        print(
+            "average great circle distance of successive samples: "
+            f"{np.mean(d):.2f} ({method})"
+        )
 
         # plot distance as histogram
-        bins = ax.hist(d, bins=bins, density=True, alpha=0.3,
-                       color='k', histtype='stepfilled')[1]
+        bins = ax.hist(
+            d, bins=bins, density=True, alpha=0.3, color="k", histtype="stepfilled"
+        )[1]
         for d_mode in d_modes[:0]:
-            ax.axvline(d_mode, ls='--', color="r")
-        ax.set_xlabel(r'$\delta(x_{n+1}, x_n)$', fontsize=fs)
-        ax.set_xticks(np.linspace(0., np.pi, 3))
+            ax.axvline(d_mode, ls="--", color="r")
+        ax.set_xlabel(r"$\delta(x_{n+1}, x_n)$", fontsize=fs)
+        ax.set_xticks(np.linspace(0.0, np.pi, 3))
         ax.set_xticklabels(["0", r"$\pi/2$", r"$\pi$"])
         ax.semilogy()
     fig.tight_layout()
 
     if save_res:
         print(f"Saving geodesic distance plot..")
         fig.savefig(f"{path}/{filename}_dist.pdf", transparent=True)
 
     plt.close(fig)
 
 
 def calc_ess(runs_samples, methods, path, return_ess=True):
-    """ 
+    """
     calculates ess using the arviz library with the default 'bulk' method
-    and saves the result. This implementation implements for multidimensional 
-    target and estimates ess values per dimension using `n` chains 
+    and saves the result. This implementation implements for multidimensional
+    target and estimates ess values per dimension using `n` chains
     """
     ess_file = f"{path}_ess.pkl.gz"
 
     # load or calculate ess (and then save)
     try:
         ess = load(ess_file, gzip=True)
         print(f"Loading ESS file {ess_file}")
 
     except FileNotFoundError:
-
         # calculate ess when `n_runs=10`
         if isinstance(runs_samples, list):
             if len(runs_samples) == 10:
-
                 print(f"Calculating ESS from samples..")
                 ess = {method: None for method in methods}
 
                 for method in methods:
-
                     # samples from all runs with shape (chains, draws, dimensions)
-                    samples = np.array([draws[method]
-                                       for draws in runs_samples])
+                    samples = np.array([draws[method] for draws in runs_samples])
 
                     # estimates ESS using the arviz library per dimension
                     samples_az = az.convert_to_dataset(samples)
                     ess_dims = az.ess(samples_az, relative=True)
                     ess[method] = ess_dims.x.values
 
                 print(f"Saving ESS file {ess_file}")
```

### Comparing `geosss-0.1.3/pyproject.toml` & `geosss-0.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "geosss"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere."
 authors = ["Michael Habeck <michael.habeck@uni-jena.de>",
            "Shantanu Kodgirwar <shantanu.kodgirwar@uni-jena.de>", 
            "Mareike Hasenpflug <mareike.hasenpflug@uni-passau.de>",
            "Daniel Rudolf <daniel.rudolf@uni-passau.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/microscopic-image-analysis/geosss"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
 scipy = "^1.11.1"
 numpy = "^1.25.1"
 matplotlib = "^3.7.2"
-seaborn = "^0.12.2"
 csb = "^1.2.5"
-tsp-solver = "^0.1"
 arviz = "^0.15.1"
 pyqt5 = "^5.15.9"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.24.0"
+seaborn = "^0.12.2"
+black = "^23.7.0"
+tsp-solver = "^0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `geosss-0.1.3/PKG-INFO` & `geosss-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geosss
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere.
 Home-page: https://github.com/microscopic-image-analysis/geosss
 License: BSD-3-Clause
 Author: Michael Habeck
 Author-email: michael.habeck@uni-jena.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: BSD License
@@ -14,16 +14,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arviz (>=0.15.1,<0.16.0)
 Requires-Dist: csb (>=1.2.5,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
-Requires-Dist: seaborn (>=0.12.2,<0.13.0)
-Requires-Dist: tsp-solver (>=0.1,<0.2)
 Project-URL: Repository, https://github.com/microscopic-image-analysis/geosss
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/microscopic-image-analysis/geosss/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
```

