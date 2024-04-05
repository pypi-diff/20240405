# Comparing `tmp/mayawaves-2023.8-py3-none-any.whl.zip` & `tmp/mayawaves-2024.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 168065 bytes, number of entries: 13
+Zip file size: 169415 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 mayawaves/__init__.py
--rw-r--r--  2.0 unx    53564 b- defN 20-Feb-02 00:00 mayawaves/coalescence.py
--rw-r--r--  2.0 unx    22585 b- defN 20-Feb-02 00:00 mayawaves/compactobject.py
--rw-r--r--  2.0 unx    75754 b- defN 20-Feb-02 00:00 mayawaves/radiation.py
+-rw-r--r--  2.0 unx    55450 b- defN 20-Feb-02 00:00 mayawaves/coalescence.py
+-rw-r--r--  2.0 unx    23819 b- defN 20-Feb-02 00:00 mayawaves/compactobject.py
+-rw-r--r--  2.0 unx    80519 b- defN 20-Feb-02 00:00 mayawaves/radiation.py
 -rw-r--r--  2.0 unx   131227 b- defN 20-Feb-02 00:00 mayawaves/utils/MAYAmetadata.pkl
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 mayawaves/utils/__init__.py
--rw-r--r--  2.0 unx    19676 b- defN 20-Feb-02 00:00 mayawaves/utils/catalogutils.py
+-rw-r--r--  2.0 unx    19801 b- defN 20-Feb-02 00:00 mayawaves/utils/catalogutils.py
 -rw-r--r--  2.0 unx    27849 b- defN 20-Feb-02 00:00 mayawaves/utils/postnewtonianutils.py
--rw-r--r--  2.0 unx   144803 b- defN 20-Feb-02 00:00 mayawaves/utils/postprocessingutils.py
-?rw-r--r--  2.0 unx    43133 b- defN 20-Feb-02 00:00 mayawaves-2023.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 mayawaves-2023.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35148 b- defN 20-Feb-02 00:00 mayawaves-2023.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1091 b- defN 20-Feb-02 00:00 mayawaves-2023.8.dist-info/RECORD
-13 files, 554917 bytes uncompressed, 166253 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx   149450 b- defN 20-Feb-02 00:00 mayawaves/utils/postprocessingutils.py
+?rw-r--r--  2.0 unx    42004 b- defN 20-Feb-02 00:00 mayawaves-2024.4.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 mayawaves-2024.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35148 b- defN 20-Feb-02 00:00 mayawaves-2024.4.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1091 b- defN 20-Feb-02 00:00 mayawaves-2024.4.dist-info/RECORD
+13 files, 566445 bytes uncompressed, 167603 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: mayawaves/utils/postnewtonianutils.py
 Comment: 
 
 Filename: mayawaves/utils/postprocessingutils.py
 Comment: 
 
-Filename: mayawaves-2023.8.dist-info/METADATA
+Filename: mayawaves-2024.4.dist-info/METADATA
 Comment: 
 
-Filename: mayawaves-2023.8.dist-info/WHEEL
+Filename: mayawaves-2024.4.dist-info/WHEEL
 Comment: 
 
-Filename: mayawaves-2023.8.dist-info/licenses/LICENSE
+Filename: mayawaves-2024.4.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: mayawaves-2023.8.dist-info/RECORD
+Filename: mayawaves-2024.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mayawaves/coalescence.py

```diff
@@ -178,16 +178,16 @@
 
         return time, separation_vector
 
     @property
     def orbital_angular_momentum_unit_vector(self) -> tuple:
         """Time and orbital angular momentum unit vector over time.
 
-        Unit vector for the orbital angular momentum computed from the positions of the primary and secondary compact
-        objects.
+        Unit vector for the orbital angular momentum computed from the coordinate positions of the primary and secondary
+        compact objects.
         """
         time, separation_vector = self.separation_vector
 
         nhat = separation_vector / np.linalg.norm(separation_vector, axis=1).reshape(separation_vector.shape[0], 1)
         dnhat_dt = np.gradient(nhat, axis=0) / (np.gradient(time).reshape(nhat.shape[0], 1))
         orbital_frequency = np.cross(nhat, dnhat_dt, axis=1)
         mag_orbital_frequency = np.linalg.norm(orbital_frequency, axis=1)
@@ -195,40 +195,43 @@
         orbital_angular_momentum_unit_vector = orbital_frequency / mag_orbital_frequency.reshape(
             orbital_frequency.shape[0], 1)
 
         return time, orbital_angular_momentum_unit_vector
 
     @property
     def orbital_phase_in_xy_plane(self) -> tuple:
-        """Time and orbital phase over time in the xy plane."""
+        """Time and orbital phase over time in the xy plane computed from the coordinate positions."""
         time, separation_vector = self.separation_vector
 
         phase = np.unwrap(np.arctan2(separation_vector[:, 1], separation_vector[:, 0]))
 
         return time, phase
 
     @property
     def orbital_frequency(self) -> tuple:
         """Time and orbital frequency over time.
 
-        Compute and return the orbital frequency as a function of time, calculated from the separation between the
-        primary and secondary compact objects.
+        Compute and return the orbital frequency as a function of time, calculated from the coordinate separation
+        between the primary and secondary compact objects.
         """
         time, separation_vector = self.separation_vector
 
         nhat = separation_vector / np.linalg.norm(separation_vector, axis=1).reshape(separation_vector.shape[0], 1)
         dnhat_dt = np.gradient(nhat, axis=0) / (np.gradient(time).reshape(nhat.shape[0], 1))
         orbital_frequency = np.cross(nhat, dnhat_dt, axis=1)
         mag_orbital_frequency = np.linalg.norm(orbital_frequency, axis=1)
 
         return time, mag_orbital_frequency
 
     @property
     def average_run_speed(self) -> float:
         """Average speed of the simulation in M/hr."""
+        if "runstats" not in self.__h5_file:
+            warnings.warn('Runstats information is not available for this coalescence.')
+            return None
         speed_column = self.__h5_file["runstats"].attrs["header"].tolist().index("speed (hours^-1)")
         return float(np.mean(self.__h5_file["runstats"][:, speed_column], axis=0))
 
     @property
     def l_max(self) -> int:
         """Maximum l mode included."""
         return self.__radiation_mode_bundle.l_max
@@ -267,15 +270,15 @@
         # older versions used "Ylm_WEYLSCAL4" ascii files, newer ones are more explicit
         if source == "Ylm_WEYLSCAL4":
             source = "YLM_WEYLSCAL4_ASC"
         return source
 
     @property
     def merge_time(self) -> float:
-        """Time at which the separation goes below 1e-2"""
+        """Time at which the coordinate separation goes below 1e-2"""
         time, separation_vector = self.separation_vector
         separation_mag = np.linalg.norm(separation_vector, axis=1)
         return time[np.argmax(separation_mag < 1e-2)]
 
     @property
     def radiation_frame(self) -> str:
         """The current frame of the radiation data"""
@@ -285,14 +288,19 @@
         """Set the frame for the radiation mode decomposition.
 
         Options are center of mass drift corrected or the original, raw frame
 
         Args:
             center_of_mass_corrected (:obj:`bool`, optional): Whether to correct for center of mass drift. Default False. If false, the frame is set back to the original, raw frame.
         """
+        import sys
+        if sys.version_info.major == 3 and sys.version_info.minor > 10:
+            warnings.warn('Python version too recent to be compatible with Scri package. Unable to change the radiation frame.')
+            raise ImportError('Unable to change the radiation frame. Python version too recent to be compatible with Scri package. If you would like the ability to move to center-of-mass corrected frame, use python <= 3.10.')
+
         from mayawaves.radiation import Frame
 
         if center_of_mass_corrected:
             com_time, center_of_mass = self.center_of_mass
             if com_time is None or center_of_mass is None:
                 warnings.warn('Unable to compute center of mass and therefore unable to correct for it. Staying in the raw frame.')
                 return
@@ -374,15 +382,15 @@
 
         """
         self.radiationbundle.radius_for_extrapolation = extraction_radius
 
     def recoil_velocity(self, km_per_sec: bool = False) -> np.ndarray:
         """Kick vector of the final object
 
-        Computed from the momentum radiated in gravitational waves
+        Computed from the momentum radiated in gravitational waves.
 
         Args:
             km_per_sec (:obj:`bool`, optional): whether to report the velocity in km/s. Defaults to reporting as a fraction of c.
 
         Returns:
             np.ndarray: the recoil velocity
 
@@ -398,15 +406,17 @@
         kick_vector = -1 * total_radiated_momentum / final_horizon_mass
         if km_per_sec:
             speed_of_light_km_per_s = 299792.458
             kick_vector = kick_vector * speed_of_light_km_per_s
         return kick_vector
 
     def recoil_speed(self, km_per_sec: bool = False) -> float:
-        """Magnitude of the recoil of the final object
+        """Magnitude of the recoil of the final object.
+
+        Computed from the momentum radiated in gravitational waves.
 
         Args:
             km_per_sec (:obj:`bool`, optional): whether to report the speed in km/s. Defaults to reporting as a fraction of c.
 
         Returns:
             float: the speed of the recoil
 
@@ -429,15 +439,15 @@
             """
         return self.compact_objects[id]
 
     def separation_at_time(self, desired_time: float) -> float:
         """Separation at a given time.
 
             Computes and returns the coordinate separation between the primary and secondary compact object centers at
-            the desired time.
+            the desired time. Points from the primary object to the secondary object.
 
             Args:
                  desired_time (float): time at which to return the separation
 
             Returns:
                 float: separation at the desired time
 
@@ -451,16 +461,16 @@
             warnings.warn("Returning the separation at the earliest available time: t={t}".format(t=time[0]))
             return separation_magnitude[0]
         return separation_magnitude[np.argmax(time > desired_time)]
 
     def orbital_frequency_at_time(self, desired_time: float) -> float:
         """Orbital frequency at given time.
 
-        Compute and return the orbital frequency at the desired time, calculated from the separation between the
-        primary and secondary compact objects.
+        Compute and return the orbital frequency at the desired time, calculated from the coordinate separation between
+        the primary and secondary compact objects.
 
         Args:
             desired_time (float): time at which to return the orbital separation
 
         Returns:
             float: orbital frequency at the desired time
 
@@ -474,16 +484,16 @@
             return orbital_frequency[0]
 
         return orbital_frequency[np.argmax(time > desired_time)]
 
     def orbital_angular_momentum_unit_vector_at_time(self, desired_time: float) -> np.ndarray:
         """Orbital angular momentum unit vector at desired time.
 
-        Unit vector for the orbital angular momentum computed from the positions of the primary and secondary compact
-        objects.
+        Unit vector for the orbital angular momentum computed from the coordinate positions of the primary and secondary
+        compact objects.
 
         Args:
             desired_time (float): time at which to return the orbital separation
 
         Returns:
             numpy.ndarray: unit vector of the orbital angular momentum at the desired time
 
@@ -499,16 +509,16 @@
             return orbital_angular_momentum_unit_vector[0]
 
         return orbital_angular_momentum_unit_vector[np.argmax(time > desired_time)]
 
     def separation_unit_vector_at_time(self, desired_time: float) -> np.ndarray:
         """Separation unit vector at desired time.
 
-        Unit vector for the separation computed from the positions of the primary and secondary compact objects.
-        Points from the primary object to the secondary object.
+        Unit vector for the separation computed from the coordinate positions of the primary and secondary compact
+        objects. Points from the primary object to the secondary object.
 
         Args:
             desired_time (float): time at which to return the separation unit vector
 
         Returns:
             numpy.ndarray: unit vector of the separation at the desired time
 
@@ -518,19 +528,21 @@
         cut_index = np.argmax(time > desired_time)
         if time[cut_index] > (desired_time + 1):
             raise IOError("Can't obtain separation data at that time")
 
         nhat = separation_vector / np.linalg.norm(separation_vector, axis=1).reshape(separation_vector.shape[0], 1)
         return nhat[cut_index]
 
-    def _crop_to_four_orbits(self, start_time: float, time: np.ndarray, orbital_phase: np.ndarray,
-                             separation_magnitude: np.ndarray, data: np.ndarray) -> tuple:
-        """Crop a given timeseries to four orbits
-
-        Compute and return four orbits worth of a given timeseries, beginning at the specified start time
+    def _crop_to_three_or_four_orbits(self, start_time: float, time: np.ndarray, orbital_phase: np.ndarray,
+                                      separation_magnitude: np.ndarray, data: np.ndarray) -> tuple:
+        """Crop a given timeseries to three or four orbits, preferring four.
+
+        Compute and return four orbits worth of a given timeseries, beginning at the specified start time. If there are
+        not four orbits, it crops to three orbits. If there aren't three orbits, it returns None. The number of orbits
+        is determined by the orbital phase.
 
         Args:
             start_time (float): time at which to begin crop
             time (numpy.ndarray): time stamps associated with data
             orbital_phase (numpy.ndarray): orbital phase associated with data
             separation_magnitude (numpy.ndarray): magnitude of the separation associated with data
             data (numpy.ndarray): timeseries to be cropped
@@ -542,25 +554,26 @@
         merge_time = time[np.argmax(separation_magnitude < 0.1)]
 
         if merge_time <= 0:
             merge_time = time[-1]
 
         start_index = np.argmax(time > start_time)
 
+        three_orbits_time = time[np.argmax(orbital_phase > (6 * np.pi + orbital_phase[start_index]))]
         four_orbits_time = time[np.argmax(orbital_phase > (8 * np.pi + orbital_phase[start_index]))]
-        if four_orbits_time <= 0:
-            four_orbits_time = time[-1]
-
-        end_time = min(four_orbits_time, merge_time - 100 if merge_time > 500 else merge_time - 25)
-        end_index = np.argmax(time >= end_time)
 
-        if end_time - start_time < 50:
+        end_time = four_orbits_time
+        if end_time <= 0 or end_time > merge_time - 50:
+            end_time = three_orbits_time
+        if end_time <= 0 or end_time > merge_time - 50:
             print("There is not enough data to crop to four orbits")
             return None, None
 
+        end_index = np.argmax(time >= end_time)
+
         time = time[start_index: end_index]
         data = data[start_index: end_index]
 
         if len(time) < 1:
             print("There is not enough data to crop to four orbits")
             return None, None
 
@@ -568,15 +581,15 @@
 
     def _anomaly_from_apsis_times(self, periapsis_times: np.ndarray, apoapsis_times: np.ndarray,
                                   desired_time: float) -> float:
         """Mean anomaly based on periapsis and apoapsis times
 
         Compute and return the mean anomaly at the desired time using
         :math:`2 \pi * \frac{t - T_{prev}}{T_{next} - T_{prev}}` where :math:`T_{next}' and :math:`T_{prev}' are
-        periabsis times.
+        periapsis times.
 
         Args:
             periapsis_times (numpy.ndarray): times of periapsis
             apoapsis_times (numpy.ndarray): times of apoapsis
             desired_time (float): time at which mean anomaly should be reported
 
         Returns:
@@ -627,16 +640,18 @@
 
         return mean_anomaly
 
     def eccentricity_and_mean_anomaly_at_time(self, start_time, desired_time) -> tuple:
         """Eccentricity and mean anomaly at desired time.
 
         Compute the eccentricity and the mean anomaly using the orbital frequency as described in https://arxiv.org/abs/1810.00036.
-        Computes the eccentricity averaged over four orbits. If it is unable to fit four orbits of data succesfully, it returns
-        an estimate of the eccentricity based on the initial momentum.
+        Computes the eccentricity averaged over four orbits. If it is unable to fit four orbits of data successfully, it returns
+        an estimate of the eccentricity based on the initial momentum. Mean anomaly is defined as
+        :math:`2 \pi * \frac{t - T_{prev}}{T_{next} - T_{prev}}` where :math:`T_{next}' and :math:`T_{prev}' are
+        periapsis times.
 
         Args:
             start_time (float): time from which to begin fitting eccentricity
             desired_time (float): time at which to return the eccentricity
 
         Returns:
             tuple: averaged eccentricity over first four orbits and the mean anomaly at the desired time
@@ -659,29 +674,32 @@
         primary_dimensional_spin = self.primary_compact_object.initial_dimensional_spin
 
         if primary_dimensionless_spin is None or secondary_dimensionless_spin is None:
             return None, None
 
         # rough estimate with initial velocity
         time_momentum, momentum_vector = self.primary_compact_object.momentum_vector
+        if momentum_vector is None:
+            return -1, -1
+
         initial_momentum = momentum_vector[0]
         tangential_initial_momentum = initial_momentum[1]
         qc_tangential_momentum = pn.tangential_momentum_from_separation(separation_magnitude[0], mass_ratio,
                                                                         primary_dimensionless_spin,
                                                                         secondary_dimensionless_spin)
 
         eps = 1 - tangential_initial_momentum / qc_tangential_momentum
 
         estimated_eccentricity = abs(2 * eps - eps ** 2)
 
         if estimated_eccentricity > 0.2:
             warnings.warn("Estimated eccentricity is higher than 0.2 so the orbital frequncy fit won't be valid. Returning the eccentricity estimated from the initial momentum.")
             return estimated_eccentricity, -1
 
-        time_inspiral, orbital_frequency_inspiral = self._crop_to_four_orbits(start_time=start_time, time=time,
+        time_inspiral, orbital_frequency_inspiral = self._crop_to_three_or_four_orbits(start_time=start_time, time=time,
                                                                               orbital_phase=orbital_phase,
                                                                               separation_magnitude=separation_magnitude,
                                                                               data=orbital_frequency)
 
         if time_inspiral is None:
             warnings.warn('Unable to fit for the eccentricity. Returning the eccentricity based on newtonian estimations from initial momentum.')
             return estimated_eccentricity, -1
@@ -844,15 +862,16 @@
         except RuntimeError as e:
             warnings.warn(f"Runtime error encountered when trying to fit the orbital frequency with an eccentric ansatz. Returning the eccentricity computed using the quasi-circular fit.")
             return eccentricity_from_qc, -1
 
     def extrapolate_psi4_to_infinite_radius(self, order: int = 1, extraction_radius: float = None):
         """Calculate :math:`\Psi_4` at infinite radius by extrapolation.
 
-        Extrapolates from a finite radius to obtain :math:`\Psi_4` at infinite radius.
+        Extrapolates from a finite radius to obtain :math:`\Psi_4` at infinite radius using the method described in
+        https://arxiv.org/abs/1008.4360 and https://arxiv.org/abs/1108.4421.
 
         Args:
             order (:obj:`int`, optional): order of extraction. Defaults to 1.
             extraction_radius: radius to extrapolate from
 
         """
         if extraction_radius is not None:
@@ -899,16 +918,17 @@
         phase = self.__radiation_mode_bundle.get_psi4_phase_for_mode(l, m, extraction_radius=extraction_radius)
         time = self.__radiation_mode_bundle.get_time(extraction_radius)
         return time, amplitude, phase
 
     def strain_for_mode(self, l: int, m: int, extraction_radius: float = 0) -> tuple:
         """Real and imaginary components of strain for a given mode.
 
-        Returns the time and the plus and cross components of :math:`rh` for a given mode and extraction radius, where r is the extraction radiys. The
-        strain is the second time integral of :math:`\Psi_4`.
+        Returns the time and the plus and cross components of :math:`rh` for a given mode and extraction radius,
+        where r is the extraction radiys. The strain is the second time integral of :math:`\Psi_4` computed using
+        fixed-frequency integration.
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided,
                 extrapolates to infinite radius.
 
@@ -941,15 +961,15 @@
         time = self.__radiation_mode_bundle.get_time(extraction_radius)
         return time, plus, cross
 
     def strain_amp_phase_for_mode(self, l: int, m: int, extraction_radius: float = 0) -> tuple:
         """Amplitude and phase of strain for a given mode.
 
         Returns the time and amplitude and phase of the strain for a given mode and extraction radius. The
-        strain is the second time integral of :math:`\Psi_4`.
+        strain is the second time integral of :math:`\Psi_4` computed using fixed-frequency integration.
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided,
                 extrapolates to infinite radius.
 
@@ -979,15 +999,16 @@
         """
         return self.__radiation_mode_bundle.get_psi4_max_time_for_mode(l, m, extraction_radius)
 
     def dEnergy_dt_radiated(self, lmin: int = None, lmax: int = None, l: int = None, m: int = None,
                             extraction_radius: float = None) -> tuple:
         """Rate at which energy is radiated in gravitational waves
 
-        If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
+        Computed using the method described in https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided,
+        it computes the total sum of all modes.
 
         Args:
             lmin (:obj:`int`, optional): minumum value of l range
             lmax (:obj:`int`, optional): maximum value of l range
             l (:obj:`int`, optional): specific l value
             m (:obj:`int`, optional): specific m value
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided, extrapolates to
@@ -1014,15 +1035,16 @@
 
         return time, energydot_radiated
 
     def energy_radiated(self, lmin: int = None, lmax: int = None, l: int = None, m: int = None,
                         extraction_radius: float = None) -> tuple:
         """Cummulative nergy radiated in gravitational waves.
 
-        Returns the cumulative energy radiated. If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
+        Returns the cumulative energy radiated computed using the method described in https://arxiv.org/abs/0707.4654.
+        If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
 
         Args:
             lmin (:obj:`int`, optional): minumum value of l range
             lmax (:obj:`int`, optional): maximum value of l range
             l (:obj:`int`, optional): specific l value
             m (:obj:`int`, optional): specific m value
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided, extrapolates to
@@ -1049,15 +1071,16 @@
 
         return time, energy_radiated
 
     def dP_dt_radiated(self, lmin: int = None, lmax: int = None, l: int = None, m: int = None,
                        extraction_radius: float = None) -> tuple:
         """Derivative of linear momentum radiated.
 
-        The rate of linear momentum being radiated through gravitational waves. If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
+        The rate of linear momentum being radiated through gravitational waves, computed using the method described in
+        https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
 
         Args:
             lmin (:obj:`int`, optional): minumum value of l range
             lmax (:obj:`int`, optional): maximum value of l range
             l (:obj:`int`, optional): specific l value
             m (:obj:`int`, optional): specific m value
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided, extrapolates to
@@ -1083,16 +1106,16 @@
         time, dP_dt = self.radiationbundle.get_dP_dt_radiated(**kwargs)
         return time, dP_dt
 
     def linear_momentum_radiated(self, lmin: int = None, lmax: int = None, l: int = None, m: int = None,
                                  extraction_radius: float = None) -> tuple:
         """Cummulative inear momentum radiated.
 
-        Cummulative linear momentum radiated through gravitational waves. If no lmin, lmax, l, or m are provided, it
-        computes the total sum of all modes.
+        Cummulative linear momentum radiated through gravitational waves, computed using the method described in
+        https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
 
         Args:
             lmin (:obj:`int`, optional): minumum value of l range
             lmax (:obj:`int`, optional): maximum value of l range
             l (:obj:`int`, optional): specific l value
             m (:obj:`int`, optional): specific m value
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided,
```

## mayawaves/compactobject.py

```diff
@@ -165,30 +165,58 @@
         """All the Columns included for this compact object."""
         return [column for column in CompactObject.Column if column.header_text in self.__header_list]
 
     @property
     def initial_dimensionless_spin(self) -> np.ndarray:
         """The dimensionless spin (:math:`\pmb{a}` or :math:`\pmb{\chi} = \pmb{J}/M^2`) at the beginning of the
         simulation."""
-        return self.__initial_dimensionless_spin
+        if self.__initial_dimensionless_spin is not None:
+            return self.__initial_dimensionless_spin
+        else:
+            time, dimensionless_spin_vector = self.dimensionless_spin_vector
+            if dimensionless_spin_vector is not None and len(dimensionless_spin_vector) > 0:
+                return dimensionless_spin_vector[0]
+            else:
+                return None
 
     @property
     def initial_dimensional_spin(self) -> np.ndarray:
         """The dimensional spin (:math:`\pmb{S}` or :math:`\pmb{J}`) at the beginning of the simulation."""
-        return self.__initial_dimensional_spin
+        if self.__initial_dimensional_spin is not None:
+            return self.__initial_dimensional_spin
+        else:
+            time, dimensional_spin_vector = self.dimensional_spin_vector
+            if dimensional_spin_vector is not None and len(dimensional_spin_vector) > 0:
+                return dimensional_spin_vector[0]
+            else:
+                return None
 
     @property
     def initial_irreducible_mass(self) -> float:
         """The irreducible mass at the beginning of the simulation."""
-        return self.__initial_irreducible_mass
+        if self.__initial_irreducible_mass is not None:
+            return self.__initial_irreducible_mass
+        else:
+            time, irreducible_mass = self.irreducible_mass
+            if irreducible_mass is not None and len(irreducible_mass) > 0:
+                return irreducible_mass[0]
+            else:
+                return None
 
     @property
     def initial_horizon_mass(self) -> float:
         """The horizon mass at the beginning of the simulation."""
-        return self.__initial_horizon_mass
+        if self.__initial_horizon_mass is not None:
+            return self.__initial_horizon_mass
+        else:
+            time, horizon_mass = self.horizon_mass
+            if horizon_mass is not None and len(horizon_mass) > 0:
+                return horizon_mass[0]
+            else:
+                return None
 
     @property
     def final_dimensionless_spin(self) -> np.ndarray:
         """The last available dimensionless spin (:math:`\pmb{a}` or :math:`\pmb{\chi} = \pmb{J}/M^2`) data"""
         time, dimensionless_spin = self.dimensionless_spin_vector
         if time is None or len(time) == 0:
             return None
@@ -350,15 +378,15 @@
         time = data[:, 0]
         irreducible_mass = data[:, 1]
 
         return time, irreducible_mass
 
     @property
     def apparent_horizon_mean_curvature(self) -> tuple:
-        """The time and mean curvature over time."""
+        """The time and mean curvature of the apparent horizon over time."""
         data = self.get_data_from_columns([self.Column.TIME, self.Column.MEAN_CURVATURE])
 
         if data is None:
             return None, None
 
         time = data[:, 0]
         apparent_horizon_mean_curvature = data[:, 1]
@@ -389,15 +417,15 @@
         time = data[:, 0]
         apparent_horizon_expansion_theta_l = data[:, 1]
 
         return time, apparent_horizon_expansion_theta_l
 
     @property
     def apparent_horizon_inner_expansion_theta_n(self) -> tuple:
-        """The time and the inner expansion Theta_(n) over time."""
+        """The time and the inner expansion Theta_(n) on the apparent horizon over time."""
         data = self.get_data_from_columns([self.Column.TIME, self.Column.INNER_EXPANSION_THETA_N])
 
         if data is None:
             return None, None
 
         time = data[:, 0]
         apparent_horizon_inner_expansion_theta_n = data[:, 1]
@@ -416,15 +444,15 @@
         time = data[:, 0]
         apparent_horizon_minimum_radius = data[:, 1]
 
         return time, apparent_horizon_minimum_radius
 
     @property
     def apparent_horizon_maximum_radius(self) -> tuple:
-        """The time and maximum horizon radius over time."""
+        """The time and maximum apparent horizon radius over time."""
         data = self.get_data_from_columns([self.Column.TIME, self.Column.MAX_RADIUS])
 
         if data is None:
             return None, None
 
         time = data[:, 0]
         apparent_horizon_maximum_radius = data[:, 1]
@@ -447,15 +475,15 @@
         xz_plane_circumference = circumferences_data[:, 2]
         yz_plane_circumference = circumferences_data[:, 3]
 
         return time, xy_plane_circumference, xz_plane_circumference, yz_plane_circumference
 
     @property
     def apparent_horizon_mean_radius(self) -> tuple:
-        """The time and mean horizon radius overtime."""
+        """The time and mean apparent horizon radius over time."""
         data = self.get_data_from_columns([self.Column.TIME, self.Column.MEAN_RADIUS])
 
         if data is None:
             return None, None
 
         time = data[:, 0]
         apparent_horizon_mean_radius = data[:, 1]
@@ -514,16 +542,14 @@
         Args:
             desired_time (float): the time at which to return the spin
 
         Returns:
             np.ndarray: the dimensional spin vector at the desired time
 
         """
-        if desired_time == 0:
-            return self.initial_dimensional_spin
 
         spin_data = self.get_data_from_columns([self.Column.TIME, self.Column.SX, self.Column.SY,
                                                 self.Column.SZ])
 
         if spin_data is None or len(spin_data) == 0:
             warnings.warn("Spin data not available at that time.")
             return None
```

## mayawaves/radiation.py

```diff
@@ -1,18 +1,16 @@
 import warnings
 from enum import Enum
 import h5py
 import numpy as np
 import scipy.integrate
-import scri
 from scipy.ndimage import uniform_filter1d
 from scipy.signal import butter, filtfilt
 from scipy.signal.windows import blackmanharris
 import math
-from spherical_functions import LM_index
 
 
 class Frame(Enum):
     RAW = 1
     COM_CORRECTED = 2
 
 
@@ -72,14 +70,18 @@
 
         Args:
             new_frame (Frame): Frame to transform to
             time (:obj:`numpy.ndarray`, optional): Time stamps for center of mass. Only necessary if moving to center of mass corrected frame.
             center_of_mass (:obj:`numpy.ndarray`, optional): Time series of center of mass. Only necessary if moving to center of mass corrected frame.
 
         """
+        import sys
+        if sys.version_info.major == 3 and sys.version_info.minor > 10:
+            raise ImportError('Unable to change the radiation frame. Python version too recent to be compatible with Scri package. If you would like the ability to move to center-of-mass corrected frame, use python <= 3.10.')
+
         if type(new_frame) != Frame:
             warnings.warn("You must provide the frame as a Frame enum value")
             return
         for radiation_sphere in self.radiation_spheres.values():
             radiation_sphere.set_frame(new_frame, time=time, center_of_mass=center_of_mass)
         if self.__extrapolated_sphere is not None:
             self.__extrapolated_sphere.set_frame(new_frame, time=time, center_of_mass=center_of_mass)
@@ -89,15 +91,15 @@
     def radiation_spheres(self) -> dict:
         """Dictionary containing all radius -> RadiationSphere pairs"""
         return self.__radiation_spheres
 
     @property
     def extrapolated_sphere(self):
         """The RadiationSphere with extrapolated radius. All :math:`\Psi_4` data has been extrapolated to infinite
-        radius."""
+        radius using the method described in https://arxiv.org/abs/1008.4360 and https://arxiv.org/abs/1108.4421."""
         if self.__extrapolated_sphere is None:
             self.create_extrapolated_sphere()
         return self.__extrapolated_sphere
 
     @property
     def radius_for_extrapolation(self) -> float:
         """The radius from which extrapolation to infinite radius will be computed."""
@@ -132,15 +134,15 @@
     @property
     def l_max(self) -> int:
         """Maximum l mode included."""
         return max([sphere.l_max for sphere in self.radiation_spheres.values()])
 
     @property
     def included_modes(self) -> list:
-        """:math:`\Psi_4` is decomposed into spherical harmonics labeled by (l, m). This provides a list of all (l,m)
+        """:math:`\Psi_4` is decomposed using spherical harmonics labeled by (l, m). This provides a list of all (l,m)
         modes included."""
         return sorted(list({mode for sphere in self.radiation_spheres.values() for mode in sphere.included_modes}))
 
     @property
     def included_radii(self) -> list:
         """List of all extraction radii included."""
         return sorted(list(self.radiation_spheres.keys()))
@@ -270,15 +272,16 @@
             return None
         return self.radiation_spheres[extraction_radius].get_psi4_phase_for_mode(l=l, m=m)
 
     def get_strain_plus_for_mode(self, l: int, m: int, extraction_radius: float = 0) -> np.ndarray:
         """Plus component of :math:`rh` for a given mode and extraction radius.
 
         Returns the plus component of strain for a given mode and extraction radius. The strain is the second time
-        integral of :math:`\Psi_4`. If the extraction radius is 0, the data is extrapolated to infinite radius.
+        integral of :math:`\Psi_4` computed using fixed-frequency integration. If the extraction radius is 0, the data
+        is extrapolated to infinite radius.
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
             extraction_radius (:obj:`float`, optional): extraction radius for strain data. If 0, the data at infinity is
                 provided.
 
@@ -296,15 +299,16 @@
             return None
         return self.radiation_spheres[extraction_radius].get_strain_plus_for_mode(l=l, m=m)
 
     def get_strain_cross_for_mode(self, l: int, m: int, extraction_radius: float = 0) -> np.ndarray:
         """Cross component of :math:`rh` for a given mode and extraction radius.
 
         Returns the cross component of strain for a given mode and extraction radius. The strain is the second time
-        integral of :math:`\Psi_4`. If the extraction radius is 0, the data is extrapolated to infinite radius.
+        integral of :math:`\Psi_4` computed using fixed-frequency integration. If the extraction radius is 0, the data
+        is extrapolated to infinite radius.
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
             extraction_radius (:obj:`float`, optional): extraction radius for strain data. If 0, the data at infinity is
                 provided.
 
@@ -349,15 +353,16 @@
             return None
         return self.radiation_spheres[extraction_radius].get_strain_recomposed_at_sky_location(theta=theta, phi=phi)
 
     def get_strain_amplitude_for_mode(self, l: int, m: int, extraction_radius: float = 0) -> np.ndarray:
         """Amplitude of :math:`rh` for a given mode and extraction radius.
 
         Returns the amplitude of strain for a given mode and extraction radius. The strain is the second time
-        integral of :math:`\Psi_4`. If the extraction radius is 0, the data is extrapolated to infinite radius.
+        integral of :math:`\Psi_4` computed using fixed-frequency integration. If the extraction radius is 0, the data
+        is extrapolated to infinite radius.
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
             extraction_radius (:obj:`float`, optional): extraction radius for strain data. If 0, the data at infinity is
                 provided.
 
@@ -375,15 +380,16 @@
             return None
         return self.radiation_spheres[extraction_radius].get_strain_amplitude_for_mode(l=l, m=m)
 
     def get_strain_phase_for_mode(self, l: int, m: int, extraction_radius: float = 0) -> np.ndarray:
         """Phase of :math:`rh` for a given mode and extraction radius.
 
         Returns the phase of strain for a given mode and extraction radius. The strain is the second time
-        integral of :math:`\Psi_4`. If the extraction radius is 0, the data is extrapolated to infinite radius.
+        integral of :math:`\Psi_4` computed using fixed-frequency integration. If the extraction radius is 0, the data
+        is extrapolated to infinite radius.
 
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
             extraction_radius (:obj:`float`, optional): extraction radius for strain data. If 0, the data at infinity is
                 provided.
@@ -426,15 +432,16 @@
             warnings.warn("There is no data at a radiation radius of {radius}M.".format(radius=extraction_radius))
             return None
         return self.radiation_spheres[extraction_radius].get_psi4_max_time_for_mode(l=l, m=m)
 
     def get_dEnergy_dt_radiated(self, extraction_radius: float = None, **kwargs) -> tuple:
         """Rate at which energy is radiated, :math:`dE/dt`
 
-        If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
+        Uses the method described in https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided, it
+        computes the total sum of all modes.
 
         Args:
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided,
                 extrapolates to infinite radius.
             **kwargs : parameters to specify the modes you would like to sum over
 
                 Valid keyword arguments are:
@@ -464,15 +471,16 @@
         time, energydot_radiated = desired_sphere.get_dEnergy_dt_radiated(**kwargs)
 
         return time, energydot_radiated
 
     def get_energy_radiated(self, extraction_radius: float = None, **kwargs) -> tuple:
         """Cumulative radiated energy :math:`E`
 
-        If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
+        Uses the method described in https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided, it
+        computes the total sum of all modes.
 
         Args:
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided,
                 extrapolates to infinite radius.
             **kwargs : parameters to specify the modes you would like to sum over
 
                 Valid keyword arguments are:
@@ -502,15 +510,16 @@
         time, energy_radiated = desired_sphere.get_energy_radiated(**kwargs)
 
         return time, energy_radiated
 
     def get_dP_dt_radiated(self, extraction_radius: float = None, **kwargs) -> tuple:
         """Rate at which linear momentum is radiated
 
-        Rate at which linear momentum is radiated through gravitational waves. If no lmin, lmax, l, or m are provided,
+        Rate at which linear momentum is radiated through gravitational waves, computed using the method described in
+        https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided,
         it computes the total sum of all modes.
 
         Args:
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided,
                 extrapolates to infinite radius.
             **kwargs : parameters to specify the modes you would like to sum over
 
@@ -541,15 +550,16 @@
         time, dP_dt_radiated = desired_sphere.get_dP_dt_radiated(**kwargs)
 
         return time, dP_dt_radiated
 
     def get_linear_momentum_radiated(self, extraction_radius: float = None, **kwargs) -> tuple:
         """Linear momentum radiated
 
-        Cummulative linear momentum radiated through gravitational waves. If no lmin, lmax, l, or m are provided, it
+        Cummulative linear momentum radiated through gravitational waves, computed using the method described in
+        https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided, it
         computes the total sum of all modes.
 
         Args:
             extraction_radius (:obj:`float`, optional): radius for gravitational wave extraction. If not provided,
                 extrapolates to infinite radius.
             **kwargs : parameters to specify the modes you would like to sum over
 
@@ -582,15 +592,16 @@
         return time, linear_momentum_radiated
 
     def create_extrapolated_sphere(self, order: int = 1):
         """Create a RadiationSphere object extrapolated from the RadiationSphere at the provided radius for
         extrapolation.
 
         Extrapolate the :math:`\Psi_4` of all RadiationModes in the RadiationSphere at the set radius for extrapolation
-        to infinite radius and create and store a new RadiationSphere with those extrapolated RadiationModes.
+        to infinite radius and create and store a new RadiationSphere with those extrapolated RadiationModes. Uses
+        the extrapolation method described in https://arxiv.org/abs/1008.4360 and https://arxiv.org/abs/1108.4421.
 
         Args:
             order (:obj:`int`, optional): the extrapolation order. Defaults to 1.
 
         """
         radiation_sphere = self.radiation_spheres[self.radius_for_extrapolation]
         extrap_sphere = radiation_sphere.get_extrapolated_sphere(order=order)
@@ -672,14 +683,19 @@
         Args:
             new_frame (Frame): Frame to transform to
             time (:obj:`numpy.ndarray`, optional): Time stamps for center of mass. Only necessary if moving to center of mass corrected frame and not providing alpha and beta.
             center_of_mass (:obj:`numpy.ndarray`, optional): Time series of center of mass. Only necessary if moving to center of mass corrected frame and not providing alpha and beta.
             alpha (:obj:`numpy.ndarray`, optional): Offset for center of mass correction. Only necessary if moving to center of mass corrected frame and not providing the center of mass timeseries.
             beta (:obj:`numpy.ndarray`, optional): Boost for center of mass correction. Only necessary if moving to center of mass corrected frame and not providing the center of mass timeseries.
         """
+        import sys
+        if sys.version_info.major == 3 and sys.version_info.minor > 10:
+            raise ImportError(
+                'Unable to change the radiation frame. Python version too recent to be compatible with Scri package. If you would like the ability to move to center-of-mass corrected frame, use python <= 3.10.')
+
         if type(new_frame) != Frame:
             warnings.warn('You must provide the new frame as a Frame enum')
             return
 
         if alpha is not None and beta is not None:
             self.__alpha = alpha
             self.__beta = beta
@@ -691,14 +707,19 @@
 
     @property
     def modes(self) -> dict:
         """Dictionary containing all the (l, m) -> RadiationMode objects in the current frame."""
         if self.frame == Frame.RAW:
             return self.raw_modes
         if self.frame == Frame.COM_CORRECTED:
+            import sys
+            if sys.version_info.major == 3 and sys.version_info.minor > 10:
+                raise ImportError(
+                    'Unable to return modes in center-of-mass corrected frame. Python version too recent to be compatible with Scri package. If you would like the ability to move to center-of-mass corrected frame, use python <= 3.10.')
+
             if self.__com_corrected_modes is None:
                 self.__frame = Frame.RAW
                 self._generate_com_corrected_modes()
                 self.__frame = Frame.COM_CORRECTED
             if self.__com_corrected_modes is None:  # if it's Still none after trying to set it
                 warnings.warn("Unable to correct for center of mass offset. Remaining in original frame.")
                 self.__frame = Frame.RAW
@@ -723,14 +744,19 @@
             return 0
         return max([l for l, m in self.included_modes])
 
     @property
     def time(self) -> np.ndarray:
         """Time array associated with all timeseries provided by this RadiationSphere."""
         if self.frame == Frame.COM_CORRECTED:
+            import sys
+            if sys.version_info.major == 3 and sys.version_info.minor > 10:
+                raise ImportError(
+                    'Unable to return time in center-of-mass corrected frame. Python version too recent to be compatible with Scri package. If you would like the ability to move to center-of-mass corrected frame, use python <= 3.10.')
+
             return self.__com_corrected_time
         return self.__time
 
     @property
     def radius(self) -> float:
         """Radius at which the :math:`\Psi_4` data was extracted."""
         return self.__radius
@@ -823,15 +849,15 @@
             warnings.warn("There is no l={l}, m={m} mode for this radiation sphere".format(l=l, m=m))
             return
         return self.modes[(l, m)].psi4_phase
 
     def get_strain_plus_for_mode(self, l: int, m: int) -> np.ndarray:
         """Plus component of :math:`rh` for a given mode.
 
-        The strain is the second time integral of :math:`\Psi_4`.
+        The strain is the second time integral of :math:`\Psi_4` computed using fixed-frequency integration.
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
 
         Returns:
             numpy.ndarray: :math:`rh_+` for a given mode
@@ -842,15 +868,15 @@
             return None
 
         return self.modes[(l, m)].strain_plus
 
     def get_strain_cross_for_mode(self, l: int, m: int) -> np.ndarray:
         """Cross component of :math:`rh` for a given mode.
 
-        The strain is the second time integral of :math:`\Psi_4`.
+        The strain is the second time integral of :math:`\Psi_4` computed using fixed-frequency integration.
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
 
         Returns:
             numpy.ndarray: :math:`rh_{\\times}` for a given mode
@@ -861,15 +887,15 @@
             return None
 
         return self.modes[(l, m)].strain_cross
 
     def get_strain_amplitude_for_mode(self, l: int, m: int) -> np.ndarray:
         """Amplitude of :math:`rh` for a given mode.
 
-        The strain is the second time integral of :math:`\Psi_4`.
+        The strain is the second time integral of :math:`\Psi_4` computed using fixed-frequency integration.
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
 
         Returns:
             numpy.ndarray: amplitude of :math:`rh` for a given mode
@@ -880,15 +906,15 @@
             return
 
         return self.modes[(l, m)].strain_amplitude
 
     def get_strain_phase_for_mode(self, l: int, m: int) -> np.ndarray:
         """Phase of :math:`rh` for a given mode.
 
-        The strain is the second time integral of :math:`\Psi_4`.
+        The strain is the second time integral of :math:`\Psi_4` computed using fixed-frequency integration.
 
         Args:
             l (int): l value of mode
             m (int): m value of mode
 
         Returns:
             numpy.ndarray: phase of :math:`rh` for a given mode
@@ -951,15 +977,16 @@
             warnings.warn("There is no l={l}, m={m} mode for this radiation sphere".format(l=l, m=m))
             return
         return self.modes[(l, m)].psi4_max_time
 
     def get_dEnergy_dt_radiated(self, **kwargs) -> tuple:
         """Rate at which energy is radiated, :math:`dE/dt`
 
-        If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
+        Uses the method described in https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided, it
+        computes the total sum of all modes.
 
         Args:
             **kwargs : parameters to specify the modes you would like to sum over
 
                 Valid keyword arguments are:
 
                 lmin (:obj:`int`, optional): minumum value of l range
@@ -1015,15 +1042,16 @@
                 energydot_radiated_total += curr_mode_denergy_radiated
 
         return time, energydot_radiated_total
 
     def get_energy_radiated(self, **kwargs) -> tuple:
         """Cumulative radiated energy :math:`E`
 
-        If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
+        Uses the method described in https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided, it
+        computes the total sum of all modes.
 
         Args:
             **kwargs : parameters to specify the modes you would like to sum over
 
                 Valid keyword arguments are:
 
                 lmin (:obj:`int`, optional): minumum value of l range
@@ -1079,16 +1107,16 @@
                 energy_radiated_total += curr_mode_energy_radiated
 
         return time, energy_radiated_total
 
     def get_dP_dt_radiated(self, **kwargs) -> tuple:
         """Rate at which linear momentum is radiated
 
-        Rate at which linear momentum is radiated through gravitational waves. If no lmin, lmax, l, or m are provided,
-        it computes the total sum of all modes.
+        Rate at which linear momentum is radiated through gravitational waves, computed using the method described in
+        https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
 
         Args:
             **kwargs : parameters to specify the modes you would like to sum over
 
                 Valid keyword arguments are:
 
                 lmin (:obj:`int`, optional): minumum value of l range
@@ -1137,16 +1165,16 @@
                 dP_dt_total += self.modes[(l, m)].dP_dt_radiated
 
         return self.time, dP_dt_total
 
     def get_linear_momentum_radiated(self, **kwargs) -> tuple:
         """Linear momentum radiated
 
-        Linear momentum radiated through gravitational waves. If no lmin, lmax, l, or m are provided, it computes the
-        total sum of all modes.
+        Linear momentum radiated through gravitational waves computed using the method described in
+        https://arxiv.org/abs/0707.4654. If no lmin, lmax, l, or m are provided, it computes the total sum of all modes.
 
         Args:
             **kwargs : parameters to specify the modes you would like to sum over
 
                 Valid keyword arguments are:
 
                 lmin (:obj:`int`, optional): minumum value of l range
@@ -1199,15 +1227,16 @@
 
         return self.time, linear_momentum_total
 
     def get_extrapolated_sphere(self, order: int = 1):
         """RadiationSphere object extrapolated from this RadiationSphere to infinite radius.
 
         Extrapolate the :math:`\Psi_4` of all RadiationModes in this RadiationSphere to infinite radius and create and
-        return a new RadiationSphere with those extrapolated RadiationModes.
+        return a new RadiationSphere with those extrapolated RadiationModes. Uses the method described in
+        https://arxiv.org/abs/1008.4360 and https://arxiv.org/abs/1108.4421.
 
         Args:
             order (:obj:`int`, optional): the extrapolation order. Defaults to 1.
 
         Returns:
             RadiationSphere: A RadiationSphere with the same properties as this one but with :math:`\Psi_4` extrapolated
             to infinite radius.
@@ -1223,24 +1252,36 @@
                 temp_modes[mode_tuple] = extrap_mode
 
         if len(temp_modes.keys()) == 0:
             return None
         extrapolated_sphere = RadiationSphere(mode_dict=temp_modes, time=np.array(self.__time), radius=self.radius,
                                               extrapolated=True)
         if self.frame != Frame.RAW:
+            import sys
+            if sys.version_info.major == 3 and sys.version_info.minor > 10:
+                raise ImportError(
+                    'Unable to set center-of-mass corrected frame. Python version too recent to be compatible with Scri package. If you would like the ability to move to center-of-mass corrected frame, use python <= 3.10.')
+
             extrapolated_sphere.set_frame(self.frame, alpha=self.__alpha, beta=self.__beta)
 
         return extrapolated_sphere
 
-    def _scri_waveform_modes_object(self) -> scri.WaveformModes:
+    def _scri_waveform_modes_object(self):
         """Create and return a Scri WaveformModes object containing the data for this extraction sphere.
 
+        For more information on scri objects, refer to https://scri.readthedocs.io.
+
         Returns: A Scri WaveformModes object
 
         """
+        import sys
+        if sys.version_info.major == 3 and sys.version_info.minor > 10:
+            raise ImportError(
+                'Unable to create scri waveform modes object. Python version too recent to be compatible with Scri package. If you would like the ability to move to center-of-mass corrected frame, use python <= 3.10.')
+
         from scri import WaveformModes
         from scri import h as scri_h
         from scri import Inertial
 
         l_min = 2
         l_max = self.l_max
 
@@ -1274,14 +1315,19 @@
         """Set the offset and boost for center of mass drift correction
 
         Args:
             com_time (np.ndarray): time stamps for the center of mass data
             center_of_mass (np.ndarray): timeseries of center of mass
 
         """
+        import sys
+        if sys.version_info.major == 3 and sys.version_info.minor > 10:
+            raise ImportError(
+                'Unable to convert to center-of-mass corrected frame. Python version too recent to be compatible with Scri package. If you would like the ability to move to center-of-mass corrected frame, use python <= 3.10.')
+
         com_time = com_time + self.radius
         t_max = np.max(com_time)
         ti = 0.1 * t_max
         tf = 0.9 * t_max
 
         idx_min = np.argmax(com_time >= ti)
         idx_max = np.argmax(com_time >= tf)
@@ -1296,16 +1342,23 @@
         # calculate alpha and beta with the Newtonian approach
         self.__alpha = (4 * (tf ** 2 + tf * ti + ti * 2) * x0 - 6 * (tf + ti) * xt0) / (tf - ti) ** 2
         self.__beta = (12 * xt0 - 6 * (tf + ti) * x0) / (tf - ti) ** 2
 
     def _generate_com_corrected_modes(self):
         """Create a dictionary of RadiationModes in a frame which has corrected for center of mass drift.
 
-        Uses scri to perform the transformation.
+        Uses scri to perform the transformation. For more information on scri, refer to https://scri.readthedocs.io.
         """
+        import sys
+        if sys.version_info.major == 3 and sys.version_info.minor > 10:
+            raise ImportError(
+                'Unable to return modes in center-of-mass corrected frame. Python version too recent to be compatible with Scri package. If you would like the ability to move to center-of-mass corrected frame, use python <= 3.10.')
+
+        from spherical_functions import LM_index
+
         scri_waveform_object = self._scri_waveform_modes_object()
         if scri_waveform_object is None:
             return
 
         scri_waveform_object = scri_waveform_object.transform(space_translation=self.__alpha,
                                                               boost_velocity=self.__beta)
         time = scri_waveform_object.t
@@ -1460,40 +1513,42 @@
         :math:`\\textrm{tan}^{-1}( \mathcal{Im}(\Psi_4) / \mathcal{Re}(\Psi_4) )`."""
         if self.__psi4_phase is None:
             self.__psi4_phase = -1 * np.unwrap(np.arctan2(self.psi4_imaginary, self.psi4_real))
         return self.__psi4_phase
 
     @property
     def strain_plus(self) -> np.ndarray:
-        """The plus component of :math:`rh` as a timeseries. The strain is computed as the second time integral of
-        :math:`\Psi_4`."""
+        """The plus component of :math:`rh` as a timeseries. The strain is the second time integral of
+        :math:`\Psi_4` computed using fixed-frequency integration."""
         if self.__strain_plus is None:
             self.compute_and_store_strain()
         return self.__strain_plus
 
     @property
     def strain_cross(self) -> np.ndarray:
-        """The cross component of :math:`rh` as a timeseries. The strain is computed as the second time integral of
-        :math:`\Psi_4`."""
+        """The cross component of :math:`rh` as a timeseries. The strain is the second time integral of
+        :math:`\Psi_4` computed using fixed-frequency integration."""
         if self.__strain_cross is None:
             self.compute_and_store_strain()
         return self.__strain_cross
 
     @property
     def strain_amplitude(self) -> np.ndarray:
         """The amplitude of :math:`rh` as a timeseries, computed from the real and imaginary parts as
-        :math:`\sqrt{\mathcal{Re}(rh)^2 + \mathcal{Im}(rh)^2}`."""
+        :math:`\sqrt{\mathcal{Re}(rh)^2 + \mathcal{Im}(rh)^2}`. The strain is the second time integral of
+        :math:`\Psi_4` computed using fixed-frequency integration."""
         if self.__strain_amplitude is None:
             self.__strain_amplitude = np.sqrt(np.power(self.strain_plus, 2) + np.power(self.strain_cross, 2))
         return self.__strain_amplitude
 
     @property
     def strain_phase(self) -> np.ndarray:
         """The phase of :math:`rh` as a timeseries, computed from the real and imaginary parts as
-        :math:`\\textrm{tan}^{-1}( \mathcal{Im}(rh) / \mathcal{Re}(rh) )`."""
+        :math:`\\textrm{tan}^{-1}( \mathcal{Im}(rh) / \mathcal{Re}(rh) )`. The strain is the second time integral of
+        :math:`\Psi_4` computed using fixed-frequency integration."""
         if self.__strain_phase is None:
             self.__strain_phase = -1 * np.unwrap(np.arctan2(self.strain_cross, self.strain_plus))
         return self.__strain_phase
 
     @property
     def radiation_sphere(self) -> RadiationSphere:
         """The RadiationSphere this mode is associated with."""
@@ -1502,20 +1557,21 @@
     @radiation_sphere.setter
     def radiation_sphere(self, radiation_sphere: RadiationSphere):
         """Set the radiation sphere this mode is associated with."""
         self.__radiation_sphere = radiation_sphere
 
     @property
     def psi4_omega(self):
-        """The frequency of :math:`\Psi_4`."""
+        """The frequency of :math:`\Psi_4` computed as the time derivative of the phase."""
         return np.gradient(self.psi4_phase, self.time)
 
     @property
     def omega_start(self):
-        """The starting frequency of :math:`\Psi_4`."""
+        """The starting frequency of :math:`\Psi_4` where the frequency is computed as the time derivative of the
+        phase."""
         start_time = self.time[0]
         end_time = start_time + 30
         if end_time > self.time[-1]:
             warnings.warn('There is not sufficient data to compute the starting frequency.')
             return None
         filter_size = np.argmax(self.time > end_time).squeeze()
         omega_rolling_average = uniform_filter1d(self.psi4_omega, size=filter_size)
@@ -1643,15 +1699,16 @@
         Pdot = self.dP_dt_radiated
         linear_momentum_radiated = scipy.integrate.cumulative_trapezoid(Pdot, self.time, initial=0, axis=0)
         return linear_momentum_radiated
 
     def compute_and_store_strain(self):
         """Computes and stores the strain data from the :math:`\Psi_4` data.
 
-        Computes the strain using the fourier transform method to compute the double time integral of :math:`\Psi_4`.
+        Computes the strain using the fixed-frequency integration method to compute the double time integral of
+        :math:`\Psi_4` using the fourier transform.
 
         """
         if self.l_value != 2 or self.m_value != 2:
             if self.radiation_sphere is None:
                 warnings.warn(
                     "This mode is not l=2, m=2 and does not have an radiation sphere. Cannot compute necessary \
                     quantities to compute strain.")
@@ -1755,15 +1812,16 @@
         self.__strain_plus = strain_plus
         self.__strain_cross = strain_cross
 
     def get_mode_with_extrapolated_radius(self, order: int = 1):
         """RadiationMode object extrapolated from this RadiationMode to infinite radius.
 
         Extrapolate the :math:`\Psi_4` of this RadiationMode to infinite radius and create and return a new
-        RadiationMode with that :math:`\Psi_4` data.
+        RadiationMode with that :math:`\Psi_4` data. Uses the method described in
+        https://arxiv.org/abs/1008.4360 and https://arxiv.org/abs/1108.4421.
 
         Args:
             order (:obj:`int`, optional): the extrapolation order. Defaults to 1.
 
         Returns:
             RadiationMode: A RadiationMode with the same properties as this one but with :math:`\Psi_4` extrapolated to
             infinite radius.
```

## mayawaves/utils/catalogutils.py

```diff
@@ -97,26 +97,27 @@
         """List of all simulations/waveforms with no spin."""
         nonspinning_simulations = self.df[(np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_1.value]) < 1e-3) &
                                           (np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_2.value]) < 1e-3)]
         return list(nonspinning_simulations.index)
 
     @property
     def aligned_spin_simulations(self):
-        """List of all simulations/waveforms with aligned spin."""
+        """List of all simulations/waveforms with spins aligned or anti-aligned with the orbital angular momentum."""
         aligned_spin_simulations = self.df[(np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_X_1.value]) < 1e-3) &
                                            (np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_Y_1.value]) < 1e-3) &
                                            (np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_X_2.value]) < 1e-3) &
                                            (np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_Y_2.value]) < 1e-3) &
                                            ((np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_1.value]) >= 1e-3) | (
                                                    np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_2.value]) >= 1e-3))]
         return list(aligned_spin_simulations.index)
 
     @property
     def precessing_simulations(self):
-        """List of all simulations/waveforms with precessing spin."""
+        """List of all simulations/waveforms with precessing spins (spins not aligned with the orbital angular
+        momentum)."""
         precessing_spin_simulations = self.df[(np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_X_1.value]) >= 1e-3) |
                                               (np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_Y_1.value]) >= 1e-3) |
                                               (np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_X_2.value]) >= 1e-3) |
                                               (np.abs(self.df[Parameter.DIMENSIONLESS_SPIN_Y_2.value]) >= 1e-3)]
         return list(precessing_spin_simulations.index)
 
     def _check_input(self, param: Parameter, value: float) -> bool:
@@ -192,29 +193,30 @@
         for param in Parameter:
             if type(self.df.loc[catalog_id][param.value]) == str:
                 print('{0:20}  {1}'.format(param.value, self.df.loc[catalog_id][param.value]))
             else:
                 print('{0:20}  {1}'.format(param.value, format(self.df.loc[catalog_id][param.value], "0.4f")))
 
     def spin_magnitudes_for_simulation(self, name: str) -> tuple:
-        """Calculates spin magnitude for each object in the binary system and returns a tuple with individual spin magnitudes.
+        """Calculates spin magnitude for each object in the binary system and returns a tuple with individual spin
+        magnitudes.
 
         Args:
             name (str): simulation/waveform name
 
         Returns:
             tuple: spin of the primary object, spin of the secondary object
 
         """
 
         simulation = self.df.loc[name]
         return simulation[Parameter.DIMENSIONLESS_SPIN_1.value], simulation[Parameter.DIMENSIONLESS_SPIN_2.value]
 
     def get_simulations_with_parameters(self, params: list, values: list, tol: list = None) -> list:
-        """This function takes in a list of parameters, their correspnding values and tolerances (optional, 0.0001
+        """Takes in a list of parameters, their corresponding values and tolerances (optional, 0.0001
         if not provided) and returns all the waveforms with those values within those tolerances.
 
         Args:
             params (list): list of parameters
             values (list): list of corresponding values
             tol (:obj:`list`, optional): list of tolerances. If not provided, tolerances of 0.0001 will be used.
 
@@ -386,15 +388,15 @@
             print(f"Minimum {p2.value}: {min(p2_array)}, maximum {p2.value}: {max(p2_array)}")
 
         else:
             print("Only the following parameters can be plotted")
             print(*Parameter, sep="\n")
 
     def download_waveforms(self, waveforms: list, save_wf_path, safety: bool = True, lvcnr_format: bool = False):
-        """Downloads a list of waveform ids from the MAYA Catalog. By default, they are downloaded in the
+        """Downloads waveforms from the MAYA Catalog given a list of waveform ids. By default, they are downloaded in the
         MAYA format, but they can also be downloaded in the lvc-nr format (https://arxiv.org/abs/1703.01076).
 
         Args:
             waveforms (list): list of waveforms to download
             save_wf_path (str): where to save the downloaded waveforms
             safety (:obj:`bool`, optional): whether to request verification if the total size of waveforms exceeds 10 GB.
                 Defaults to True.
```

## mayawaves/utils/postprocessingutils.py

```diff
@@ -564,15 +564,21 @@
         with open(list(filepaths.values())[0][0]) as f:
             for line in f:
                 if line.strip() == '#':
                     break
                 header_info = header_info + line
 
         compact_object_count = None
-        parfile_content = parameter_file_group.attrs['par_content']
+        if 'par_content' in parameter_file_group.attrs:
+            parfile_content = parameter_file_group.attrs['par_content']
+        elif 'rpar_content' in parameter_file_group.attrs:
+            parfile_content = parameter_file_group.attrs['rpar_content']
+        else:
+            warnings.warn('No parameter file information. Unable to read QuasiLocalMeasures data.')
+            return
         for line in parfile_content.splitlines():
             if 'QuasiLocalMeasures::num_surfaces' in line:
                 compact_object_count = int(line.split('=')[-1].strip())
 
         if compact_object_count == None:
             return compact_object_dict
 
@@ -1035,50 +1041,96 @@
     Returns:
         str: simulation name constructed from the directory name
 
     """
     simulation_name = raw_directory.split('/')[-1]
     return simulation_name
 
+def _get_parameter_file_name_and_content(raw_directory: str) -> tuple:
+    """Store the parameter file in the h5 file
 
-def _parameter_file_name_base(raw_directory: str) -> str:
-    """Base name from the parameter file
-
-    From the raw directory, compute the base of the parameter file name, whether it be a .rpar or .par file.
+    Search for .rpar and .par files and store in a dictionary
 
     Args:
         raw_directory (str): the directory that contains all simulation data
 
     Returns:
-        str: the base name of the parameter file
+        tuple: base name of the parameter file and a dictionary containing the rpar and par content
 
     """
+    parfile_name = None
+    parfile_dict = {}
+
+    # check if SIMFACTORY directory exists
+    rpar_file = None
+    par_file = None
     if os.path.isdir(os.path.join(raw_directory, "SIMFACTORY/par")):
-        parameter_files = glob.glob(os.path.join(raw_directory, "SIMFACTORY/par/*.rpar")) + glob.glob(
-            os.path.join(raw_directory, "SIMFACTORY/par/*.par"))
-        if len(parameter_files) > 0:  # if there is an rpar file
-            parameter_file = parameter_files[0]
-            parfile_name = parameter_file.split('/')[-1]
-            parfile_name_base = parfile_name[:parfile_name.rfind('.')]
-            return parfile_name_base
+        files_with_rpar = glob.glob(os.path.join(raw_directory, "SIMFACTORY/par/*.rpar"))
+        if len(files_with_rpar) > 0:  # if there is an rpar file
+            rpar_file = files_with_rpar[0]
+        files_with_par = glob.glob(os.path.join(raw_directory, "SIMFACTORY/par/*.par"))
+        if len(files_with_par) > 0:  # if there is a par file
+            par_file = files_with_par[0]
 
-    output_directories, _ = _ordered_output_directories(raw_directory)
-    output_directories.reverse()  # most recent output directory is first now
+    # if we haven't found a par file or a rpar file
+    if rpar_file is None or par_file is None:
+        output_directories, _ = _ordered_output_directories(raw_directory)
+        output_directories.reverse()  # most recent output directory is first now
+
+        for output_dir in output_directories:
+            if rpar_file is None:
+                files_with_rpar = glob.glob(os.path.join(output_dir, "*.rpar"))
+                if len(files_with_rpar) > 0:  # if there is a rpar file
+                    rpar_file = files_with_rpar[0]
+            if par_file is None:
+                files_with_par = glob.glob(os.path.join(output_dir, "*.par"))
+                if len(files_with_par) > 0:  # if there is a par file
+                    par_file = files_with_par[0]
+
+            if rpar_file is not None and par_file is not None:
+                break
+
+    # if we never found a parameter file
+    if rpar_file is None and par_file is None:
+        warnings.warn("Unable to locate a .rpar or .par file in this simulation directory.")
+        return None, None
 
-    for output_dir in output_directories:
-        parameter_files = glob.glob(os.path.join(output_dir, "*.rpar")) + glob.glob(os.path.join(output_dir, "*.par"))
-        if len(parameter_files) > 0:  # if there is an rpar file
-            parameter_file = parameter_files[0]
-            parfile_name = parameter_file.split('/')[-1]
-            parfile_name_base = parfile_name[:parfile_name.rfind('.')]
-            return parfile_name_base
-
-    warnings.warn(
-        "Unable to find a parameter file. Cannot determine parameter file name. Will assume same as simulation name.")
-    return _simulation_name(raw_directory)
+    created_par = False
+
+    # store the rpar file if it exists and create parfile
+    if rpar_file is not None:
+        rpar_name = rpar_file.split('/')[-1]
+        rpar_name_base = rpar_name[:rpar_name.rfind('.')]
+        parfile_name = rpar_name_base
+        with open(rpar_file, 'r') as f:
+            content = f.read()
+        parfile_dict['rpar_content'] = content
+        if par_file is None:
+            temporary_rpar = rpar_file[:rpar_file.rfind('/') + 1] + "temp.rpar"
+            par_file = rpar_file[:rpar_file.rfind('/') + 1] + "temp.par"
+            with open(temporary_rpar, 'w') as f:
+                f.write(parfile_dict['rpar_content'])
+            os.system(f'chmod +x {temporary_rpar}')
+            os.system('%s' % temporary_rpar)
+            created_par = True
+            os.remove(temporary_rpar)
+
+    # store the par file
+    if parfile_name is None:
+        par_name = par_file.split('/')[-1]
+        parfile_name = par_name[:par_name.rfind('.')]
+    if os.path.exists(par_file):
+        with open(par_file, 'r') as f:
+            content = f.read()
+        parfile_dict['par_content'] = content
+
+    if created_par and os.path.exists(par_file):
+        os.remove(par_file)
+
+    return parfile_name, parfile_dict
 
 
 def _ordered_output_directories(raw_directory: str) -> tuple:
     """The output directories within the raw directory, ordered.
 
     Find all the output directories within the raw directory and sort in ascending order. If the data has been
     prestitched, there aren't individual output directories.
@@ -1098,121 +1150,90 @@
     if len(output_directories) == 0:
         # pre-stitched data
         output_directories = [raw_directory]
         prestitched = True
     return output_directories, prestitched
 
 
-def _ordered_data_directories(raw_directory: str, parameter_file_name_base: str) -> list:
+def _ordered_data_directories(raw_directory: str, parameter_file: str, parameter_file_name_base: str) -> list:
     """The directories containing the simulation data files, ordered.
 
     Within each output directory is a data directory. Returns an ordered list of all the data directories. If the data
     is prestitched, this is the same as the output directory and raw directory.
 
     Args:
         raw_directory (str): the directory that contains all simulation data
         parameter_file_name_base (str): the base name of the parameter file
 
     Returns:
         list: ordered list containing the ordered data directories
 
     """
     output_directories, prestitched = _ordered_output_directories(raw_directory)
+
+    simulation_name = raw_directory.split('/')[-1]
+
     if prestitched:
         # pre-stitched data
         data_directories = output_directories
     else:
-        data_directories = [os.path.join(output_directory, parameter_file_name_base) for output_directory in
+        if parameter_file is None:
+            return None
+        data_dir_name = ""
+
+        result = re.search('IO::out_dir\s*=\s*(\S*)\s*\n', parameter_file)
+        try:
+            data_dir_name = result.group(1)
+            data_dir_name = data_dir_name.strip('"\'')
+        except:
+            warnings.warn("Can't find name of the data directory, assuming it is an empty string")
+        if data_dir_name == '\$parfile' or data_dir_name == '$parfile':
+            data_dir_name = parameter_file_name_base
+        if data_dir_name == '@SIMULATION_NAME@':
+            data_dir_name = simulation_name
+
+        data_directories = [os.path.join(output_directory, data_dir_name) for output_directory in
                             output_directories]
     return data_directories
 
-
-def _store_parameter_file(raw_directory: str, h5_file: h5py.File):
+def _store_parameter_file(parfile_dict: dict, h5_file: h5py.File):
     """Store the parameter file in the h5 file
 
-    Search for a .rpar file (or a .par file if there is no .rpar file) and store it
+    Store .rpar and .par file information
 
     Args:
-        raw_directory (str): the directory that contains all simulation data
+        parfile_dict (dict): dictionary containing the rpar and par content
         h5_file (h5py.file): the h5 file to store the parameter file in
 
     """
-    # check if SIMFACTORY directory exists
-    rpar_file = None
-    par_file = None
-    if os.path.isdir(os.path.join(raw_directory, "SIMFACTORY/par")):
-        files_with_rpar = glob.glob(os.path.join(raw_directory, "SIMFACTORY/par/*.rpar"))
-        if len(files_with_rpar) > 0:  # if there is an rpar file
-            rpar_file = files_with_rpar[0]
-        files_with_par = glob.glob(os.path.join(raw_directory, "SIMFACTORY/par/*.par"))
-        if len(files_with_par) > 0:  # if there is a par file
-            par_file = files_with_par[0]
-
-    # if we haven't found a par file or a rpar file
-    if rpar_file is None and par_file is None:
-        output_directories, _ = _ordered_output_directories(raw_directory)
-        output_directories.reverse()  # most recent output directory is first now
-
-        for output_dir in output_directories:
-            files_with_rpar = glob.glob(os.path.join(output_dir, "*.rpar"))
-            if len(files_with_rpar) > 0:  # if there is a rpar file
-                rpar_file = files_with_rpar[0]
-            files_with_par = glob.glob(os.path.join(output_dir, "*.par"))
-            if len(files_with_par) > 0:  # if there is a par file
-                par_file = files_with_par[0]
-
-            if rpar_file is not None or par_file is not None:
-                break
-
-    # if we never found a parameter file
-    if rpar_file is None and par_file is None:
-        warnings.warn("Unable to locate a .rpar or .par file in this simulation directory.")
+    if parfile_dict is None or ("par_content" not in parfile_dict and "rpar_content" not in parfile_dict):
         return
 
     parfile_group = h5_file.create_group('parfile')
-    created_par = False
 
-    # store the rpar file if it exists and create parfile
-    if rpar_file is not None:
-        with open(rpar_file, 'r') as f:
-            content = f.read()
-        parfile_group.attrs['rpar_content'] = content
-        if par_file is None:
-            temporary_rpar = rpar_file[:rpar_file.rfind('/') + 1] + "temp.rpar"
-            par_file = rpar_file[:rpar_file.rfind('/') + 1] + "temp.par"
-            with open(temporary_rpar, 'w') as f:
-                f.write(parfile_group.attrs['rpar_content'])
-            os.system(f'chmod +x {temporary_rpar}')
-            os.system('%s' % temporary_rpar)
-            created_par = True
-            os.remove(temporary_rpar)
-
-    # store the par file
-    with open(par_file, 'r') as f:
-        content = f.read()
-    parfile_group.attrs['par_content'] = content
-
-    if created_par:
-        os.remove(par_file)
+    if "par_content" in parfile_dict:
+        parfile_group.attrs['par_content'] = parfile_dict['par_content']
 
+    if "rpar_content" in parfile_dict:
+        parfile_group.attrs['rpar_content'] = parfile_dict['rpar_content']
 
-def _all_relevant_data_filepaths(raw_directory: str, parameter_file_name_base: str) -> dict:
+def _all_relevant_data_filepaths(raw_directory: str, parameter_file: str, parameter_file_name_base: str) -> dict:
     """Dictionary of all relevant data files.
 
     The dictionary points from a data type to a filename which in turn points to a list of filepaths with that filename.
 
     Args:
         raw_directory (str): the directory that contains all simulation data
         parameter_file_name_base (str): the base name of the parameter file
 
     Returns:
         dict: dictionary containing prefix -> filename -> list of filepaths to relevant files
 
     """
-    data_directories = _ordered_data_directories(raw_directory, parameter_file_name_base=parameter_file_name_base)
+    data_directories = _ordered_data_directories(raw_directory, parameter_file=parameter_file, parameter_file_name_base=parameter_file_name_base)
     relevant_data_filepaths = {"compact_object": {}, "radiative": {}, "misc": {}}
 
     # go through all output directories
     for output_directory in data_directories:
         data_path = os.path.join(output_directory, "*")
 
         # go through all datafiles in the output directory
@@ -1441,15 +1462,15 @@
         data = full_dataset[~nan_columns][:, columns[0]]
     else:
         data = full_dataset[~nan_columns][:, columns]
     return data
 
 
 def _get_dimensional_spin_from_parfile(parfile_group: h5py.Group) -> tuple:
-    """Provides the dimensional spin vectors from the parameter file.
+    """Provides the dimensional spin vectors (:math:`\pmb{S}` or :math:`\pmb{J}`) from the parameter file.
 
     Parses through the parameter file and returns the dimensional spin of both the primary and secondary compact
     objects.
 
     Args:
         parfile_group (h5py.Group): parameter file group in h5 file
 
@@ -1522,15 +1543,15 @@
         if np.isnan(spin_component):
             spin1[i] = 0
 
     return spin0, spin1
 
 
 def _get_initial_dimensional_spins(h5_file: h5py.File) -> tuple:
-    """Initial dimensional spins.
+    """Initial dimensional spins (:math:`\pmb{S}` or :math:`\pmb{J}`).
 
     Tries to get the initial dimensional spins from the compact object data. Otherwise, returns the spins set in the
     parameter file.
 
     Args:
         h5_file (h5py.File): h5 file containing all the data about the simulation
 
@@ -1569,15 +1590,15 @@
     spin1 = dimensional_spin_data_1[0].tolist()
 
     return spin0, spin1
 
 
 def _get_initial_dimensionless_spins(dimensional_spin_0: list, dimensional_spin_1: list,
                                      horizon_mass_0: float, horizon_mass_1: float):
-    """Initial dimensionless spins.
+    """Initial dimensionless spins (:math:`\pmb{a}` or :math:`\pmb{\chi} = \pmb{J}/M^2`).
 
     Computes and returns the dimensionless spins given the dimensional spins and the horizon masses.
 
     Args:
         dimensional_spin_0 (list): the dimensional spin of the primary compact object
         dimensional_spin_1 (list): the dimensional spin of the secondary compact object
         horizon_mass_0 (float): the horizon mass of the primary compact object
@@ -1623,15 +1644,16 @@
     else:
         return "aligned-spins"
 
 
 def _irreducible_mass_to_horizon_mass(irreducible_mass: float, dimensional_spin: list) -> float:
     """Convert the irreducible mass to the horizon mass.
 
-    Provided the irreducible mass and the dimensional spin, compute and return the horizon mass.
+    Provided the irreducible mass and the dimensional spin, compute and return the horizon mass as
+    :math:`M_{horizon} = sqrt(M_{irr}^2 + \frac{S^2}{4M_{irr}^2})`
 
     Args:
         irreducible_mass (float): the irreducible mass of the object
         dimensional_spin (list): the dimensional spin of the object
 
     Returns:
         float: the horizon mass of the object
@@ -1643,15 +1665,16 @@
 
     return horizon_mass
 
 
 def _horizon_mass_to_irreducible_mass(horizon_mass: float, dimensional_spin: list):
     """Convert the horizon mass to the irreducible mass.
 
-    Provided the horizon mass and the dimensional spin, compute and return the irreducible mass.
+    Provided the horizon mass and the dimensional spin, compute and return the irreducible mass as
+    :math:`M_{irr} = sqrt((M_{horizon}^2 + sqrt(M_{horizon}^4 - S^2))/2)`
 
     Args:
         horizon_mass (float): the horizon mass of the object
         dimensional_spin (list): the dimensional spin of the object
 
     Returns:
         float: the irreducible mass of the object
@@ -1747,15 +1770,15 @@
         print('using out file due to value error')
         return _get_masses_from_out_file(relevant_output_filepaths, dimensional_spin0, dimensional_spin1)
 
 
 def _get_initial_separation_from_parfile(parfile_group: h5py.Group) -> float:
     """Obtain the initial separation from the parameter file
 
-    Find the initial separation from the .rpar or .par file
+    Find the initial coordinate separation from the .rpar or .par file
 
     Args:
         parfile_group (h5py.Group): parameter file for the simulation
 
     Returns:
         float: initial separation
 
@@ -1775,15 +1798,16 @@
 
     return initial_separation
 
 
 def _get_initial_separation(h5_file: h5py.File) -> float:
     """Initial separation for the simulation.
 
-    Obtain the initial separation of the simulation either from the compact object data or from the parameter file.
+    Obtain the initial coordinate separation of the simulation either from the coordinate trajectories of the black
+    holes or from the parameter file.
 
     Args:
         h5_file (h5py.File): h5 file containing all the data about the simulation
 
     Returns:
         float: initial separation
 
@@ -1836,15 +1860,16 @@
 
     return initial_separation_mag
 
 
 def _get_initial_orbital_frequency(h5_file: h5py.File) -> float:
     """Initial orbital frequency for the simulation.
 
-    Obtain the initial orbital frequency of the simulation from the compact object data.
+    Obtain the initial orbital frequency of the simulation from the coordinate separation vector of the black holes.
+    Waits 75M for junk radiation to settle.
 
     Args:
         h5_file (h5py.File): h5 file containing all the data about the simulation
 
     Returns:
         float: orbital frequency after junk
 
@@ -1968,32 +1993,38 @@
 
     # determine the name of the simulation
     if not os.path.isdir(raw_directory):
         warnings.warn('That is not a simulation directory. Aborting.')
         return
 
     simulation_name = _simulation_name(raw_directory)
-    parameter_file_name_base = _parameter_file_name_base(raw_directory)
-
-    # get all relevant filepaths
-    relevant_data_filepaths = _all_relevant_data_filepaths(raw_directory,
-                                                           parameter_file_name_base=parameter_file_name_base)
-    relevant_output_filepaths = _all_relevant_output_filepaths(raw_directory)
+    parameter_file_name_base, parameter_file_dict = _get_parameter_file_name_and_content(raw_directory)
 
     if catalog_id is not None:
         h5_filename = os.path.join(output_directory, catalog_id + ".h5")
     else:
         h5_filename = os.path.join(output_directory, simulation_name + ".h5")
 
     # open h5file
     h5_file = h5py.File(h5_filename, 'w')
 
     # store parameter file
     print("storing parameter file")
-    _store_parameter_file(raw_directory, h5_file)
+    _store_parameter_file(parameter_file_dict, h5_file)
+
+    # get all relevant filepaths
+    if "parfile" in h5_file.keys():
+        if 'par_content'in h5_file["parfile"].attrs:
+            parameter_file = h5_file["parfile"].attrs["par_content"]
+        elif 'rpar_content'in h5_file["parfile"].attrs:
+            parameter_file = h5_file["parfile"].attrs["rpar_content"]
+        else:
+            parameter_file = None
+    relevant_data_filepaths = _all_relevant_data_filepaths(raw_directory, parameter_file, parameter_file_name_base)
+    relevant_output_filepaths = _all_relevant_output_filepaths(raw_directory)
 
     # process radiative data
     print("storing radiative information")
     _store_radiative_data(h5_file, relevant_data_filepaths)
 
     # process compact object data
     print("storing compact object information")
@@ -2025,17 +2056,21 @@
 
     """
 
     if not os.path.isdir(raw_directory):
         warnings.warn("That directory does not exist")
         return None
 
-    parameter_file_name_base = _parameter_file_name_base(raw_directory)
+    parameter_file_name_base, parameter_file_dict = _get_parameter_file_name_and_content(raw_directory)
 
-    data_directories = _ordered_data_directories(raw_directory, parameter_file_name_base=parameter_file_name_base)
+    if parameter_file_dict is None or 'par_content' not in parameter_file_dict:
+        warnings.warn('Unable to determine file structure due to lack of parameter file')
+        return None
+
+    data_directories = _ordered_data_directories(raw_directory, parameter_file=parameter_file_dict['par_content'], parameter_file_name_base=parameter_file_name_base)
     filepaths = []
 
     # go through all output directories
     for output_directory in data_directories:
         matching_filepaths = glob.glob(os.path.join(output_directory, filename))
         if len(matching_filepaths) > 0:
             filepath = glob.glob(os.path.join(output_directory, filename))[0]
@@ -2564,15 +2599,15 @@
     max_time = time[max_iter]
     return max_time
 
 
 def _get_omega_at_time(time: np.ndarray, phase: np.ndarray, initial_time: float) -> float:
     """Frequency at a given time.
 
-    Returns the frequency, the derivative of the phase with respect to time.
+    Returns the frequency, the derivative of the provided phase with respect to time.
 
     Args:
         time (numpy.ndarray): time array
         phase (numpy.ndarray): phase array
         initial_time (float): desired time
 
     Returns:
@@ -2584,15 +2619,15 @@
     omega_at_time = omega[time_index]
     return omega_at_time
 
 
 def _export_ascii_file(filename: str, data: np.ndarray, coalescence_directory: str, header: str = None):
     """Export specified data array to ascii.
 
-    Export specified data array to an ascii file of the given name with the necessary header.
+    Export specified data array to an ascii file of the given name with the provided header.
 
     Args:
         filename (str): the filename to be exported to
         data (np.ndarray): array containing the data to be exported
         coalescence_directory (str): the path to store the exported data
         header (str): the header to put at the top of the exported ascii file
 
@@ -2628,18 +2663,20 @@
         nr_techniques (:obj:`str`, optional): what techniques were used in this simulation
         comparable_simulation (:obj:`str`, optional): other similar simulations
         files_in_error_series (:obj:`str`, optional): other simulations in the same error series
         production_run (:obj:`bool`, optional): whether this is a production run. Default True.
         center_of_mass_correction (:obj:'bool', optional): whether to correct for center of mass drift. Default False.
 
     """
+    from mayawaves.radiation import Frame
     if center_of_mass_correction:
         coalescence.set_radiation_frame(center_of_mass_corrected=True)
     else:
-        coalescence.set_radiation_frame()
+        if not coalescence.radiation_frame == Frame.RAW:
+            coalescence.set_radiation_frame()
 
     initial_time_horizon = 75
     if extraction_radius != 0:
         initial_time_strain = initial_time_horizon + extraction_radius
     else:
         initial_time_strain = initial_time_horizon + coalescence.radiationbundle.radius_for_extrapolation
 
@@ -2698,28 +2735,31 @@
                             comparable_simulation, files_in_error_series, production_run)
 
         time_shift = max_time - (
             coalescence.radiationbundle.radius_for_extrapolation if extraction_radius == 0 else extraction_radius)
         _store_compact_object_timeseries_data(coalescence, lal_h5_file, lvc_format, time_shift, initial_time_horizon)
 
         lal_h5_file.close()
-        coalescence.set_radiation_frame()
+        if coalescence.radiation_frame != Frame.RAW:
+            coalescence.set_radiation_frame()
 
     except Exception as e:
         lal_h5_file.close()
-        coalescence.set_radiation_frame()
+        if coalescence.radiation_frame != Frame.RAW:
+            coalescence.set_radiation_frame()
         raise e
 
     if raise_mode_error:
-        coalescence.set_radiation_frame()
+        if coalescence.radiation_frame != Frame.RAW:
+            coalescence.set_radiation_frame()
         raise IOError(f"Data is missing for one of the included modes")
 
 
 def low_pass_filter(time: np.ndarray, data: np.ndarray, low_pass_freq_cutoff: float) -> np.ndarray:
-    """Filter out high frequency noise
+    """Filter out high frequency noise using a butter filter.
 
     Args:
         time (numpy.ndarray): time stamps associated with data
         data (numpy.ndarray): data to filter
         low_pass_freq_cutoff (float): frequency cutoff to use with butter filter
 
     Returns:
@@ -2734,15 +2774,16 @@
     b, a = butter(4, Wn, analog=False)
     filtered = filtfilt(b, a, data, axis=0)
 
     return filtered
 
 
 def determine_lvc_format(coalescence: Coalescence, initial_horizon_time: float) -> int:
-    """Determine the LVC format number based upon the data available from the simulation
+    """Determine the LVC format number based upon the data available from the simulation and the definitions in
+    https://arxiv.org/abs/1703.01076
 
     Args:
         coalescence (Coalescence): the Coalescence object being exported
         initial_horizon_time (float): the time for initial data at the horizon
 
     Returns:
         int: the LVC format (1, 2, 3)
@@ -3043,69 +3084,88 @@
             current_time - 0.01)
     else:
         final_horizon_mass = coalescence.final_compact_object.final_horizon_mass
         final_dimensionless_spin = coalescence.final_compact_object.final_dimensionless_spin
 
     # Format information to be printed to summary.txt:
     # beginning includes information regarding initial data.
+    mass_ratio_string = 'NaN' if initial_mass_ratio is None else f'{initial_mass_ratio:.4f}'
+    primary_horizon_mass_string = 'NaN' if initial_primary_horizon_mass is None else f'{initial_primary_horizon_mass:.4f}'
+    secondary_horizon_mass_string = 'NaN' if initial_secondary_horizon_mass is None else f'{initial_secondary_horizon_mass:.4f}'
+    primary_spin_string = 'NaN' if initial_primary_dimensionless_spin is None else f'[{initial_primary_dimensionless_spin[0]:.4f}, {initial_primary_dimensionless_spin[1]:.4f}, {initial_primary_dimensionless_spin[2]:.4f}]'
+    secondary_spin_string = 'NaN' if initial_secondary_dimensionless_spin is None else f'[{initial_secondary_dimensionless_spin[0]:.4f}, {initial_secondary_dimensionless_spin[1]:.4f}, {initial_secondary_dimensionless_spin[2]:.4f}]'
+    separation_string = 'NaN' if initial_separation is None else f'{initial_separation:.4f}'
     beginning = f"Summary for {coalescence_name}\n" \
                 f"\nInitial Values (t=0 M):\n" \
                 f"{'-' * 70}\n" \
-                f"mass ratio:\t\t\t\t{str(initial_mass_ratio)[0:6]}\n" \
-                f"primary horizon mass:\t\t\t{str(initial_primary_horizon_mass)[0:6]}\n" \
-                f"secondary horizon mass:\t\t\t{str(initial_secondary_horizon_mass)[0:6]}\n" \
-                f"primary dimensionless spin:\t\t{[round(i, 4) for i in initial_primary_dimensionless_spin]}\n" \
-                f"secondary dimensionless spin:\t\t{[round(i, 4) for i in initial_secondary_dimensionless_spin]}\n" \
-                f"separation:\t\t\t\t{str(initial_separation)[0:6]} M\n"
+                f"mass ratio:\t\t\t\t{mass_ratio_string}\n" \
+                f"primary horizon mass:\t\t\t{primary_horizon_mass_string}\n" \
+                f"secondary horizon mass:\t\t\t{secondary_horizon_mass_string}\n" \
+                f"primary dimensionless spin:\t\t{primary_spin_string}\n" \
+                f"secondary dimensionless spin:\t\t{secondary_spin_string}\n" \
+                f"separation:\t\t\t\t{separation_string} M\n"
 
     # middle includes information regarding data at t=75 M.
     if current_time < 75:
         if coalescence.final_compact_object is None:
             middle = f"\nAfter Junk Radiation (t=75 M):\n" \
                      f"{'-' * 70}\n" \
                      f"Simulation has not yet reached t=75 M.\n"
         else:
             middle = f"\nAfter Junk Radtation (t=75 M):\n" \
                      f"{'-' * 70}\n" \
                      f"Simulation completed before reaching t=75 M.\n"
     else:
-        pds_message = f"None" if primary_dimensionless_spin is None else f"{[round(i, 4) for i in primary_dimensionless_spin]}"
-        sds_message = f"None" if secondary_dimensionless_spin is None else f"{[round(i, 4) for i in secondary_dimensionless_spin]}"
+        primary_horizon_mass_string = 'NaN' if primary_horizon_mass is None else f'{primary_horizon_mass:.4f}'
+        secondary_horizon_mass_string = 'NaN' if secondary_horizon_mass is None else f'{secondary_horizon_mass:.4f}'
+        primary_spin_string = 'NaN' if primary_dimensionless_spin is None else f'[{primary_dimensionless_spin[0]:.4f}, {primary_dimensionless_spin[1]:.4f}, {primary_dimensionless_spin[2]:.4f}]'
+        secondary_spin_string = 'NaN' if secondary_dimensionless_spin is None else f'[{secondary_dimensionless_spin[0]:.4f}, {secondary_dimensionless_spin[1]:.4f}, {secondary_dimensionless_spin[2]:.4f}]'
+        separation_string = 'NaN' if separation is None else f'{separation:.4f}'
+        separation_unit_vector_string = 'NaN' if separation_unit_vector is None else f'[{separation_unit_vector[0]:.4f}, {separation_unit_vector[1]:.4f}, {separation_unit_vector[2]:.4f}]'
+        orbital_frequency_string = 'NaN' if orbital_frequency is None else f'{orbital_frequency:.4f}'
+        orbital_angular_momentum_unit_vector_string = 'NaN' if orbital_angular_momentum_unit_vector is None else f'[{orbital_angular_momentum_unit_vector[0]:.4f}, {orbital_angular_momentum_unit_vector[1]:.4f}, {orbital_angular_momentum_unit_vector[2]:.4f}]'
+        eccentricity_string = 'NaN' if eccentricity is None else f'{eccentricity:.4f}'
         middle = f"\nAfter Junk Radiation (t=75 M):\n" \
                  f"{'-' * 70}\n" \
-                 f"primary horizon mass:\t\t\t{str(primary_horizon_mass)[0:6]}\n" \
-                 f"secondary horizon mass:\t\t\t{str(secondary_horizon_mass)[0:6]}\n" \
-                 f"primary dimensionless spin:\t\t{pds_message}\n" \
-                 f"secondary dimensionless spin:\t\t{sds_message}\n" \
-                 f"separation:\t\t\t\t{str(separation)[0:6]} M\n" \
-                 f"separation unit vector:\t\t\t{[round(i, 4) for i in separation_unit_vector]}\n" \
-                 f"orbital frequency:\t\t\t{str(orbital_frequency)[0:6]}\n" \
-                 f"orbital angular momentum unit vector:\t{[round(i, 4) for i in orbital_angular_momentum_unit_vector]}\n" \
-                 f"eccentricity:\t\t\t\t{str(eccentricity)[0:6]}\n"
+                 f"primary horizon mass:\t\t\t{primary_horizon_mass_string}\n" \
+                 f"secondary horizon mass:\t\t\t{secondary_horizon_mass_string}\n" \
+                 f"primary dimensionless spin:\t\t{primary_spin_string}\n" \
+                 f"secondary dimensionless spin:\t\t{secondary_spin_string}\n" \
+                 f"separation:\t\t\t\t{separation_string} M\n" \
+                 f"separation unit vector:\t\t\t{separation_unit_vector_string}\n" \
+                 f"orbital frequency:\t\t\t{orbital_frequency_string}\n" \
+                 f"orbital angular momentum unit vector:\t{orbital_angular_momentum_unit_vector_string}\n" \
+                 f"eccentricity:\t\t\t\t{eccentricity_string}\n"
         if primary_horizon_mass is None or secondary_horizon_mass is None or \
                 primary_dimensionless_spin is None or secondary_dimensionless_spin is None:
-            middle += r"**A 'None' value represents data that was not being tracked at t=75 M.**" + "\n"
+            middle += r"**A 'NaN' value represents data that was not being tracked at t=75 M.**" + "\n"
 
     # ending includes information regarding most recent data.
     if coalescence.final_compact_object is None:
+        time_string = 'NaN' if current_time is None else f'{current_time:.4f}'
+        separation_string = 'NaN' if current_separation is None else f'{current_separation:.4f}'
+        separation_unit_vector_string = 'NaN' if current_separation_unit_vector is None else f'[{current_separation_unit_vector[0]:.4f}, {current_separation_unit_vector[1]:.4f}, {current_separation_unit_vector[2]:.4f}]'
+        orbital_frequency_string = 'NaN' if current_orbital_frequency is None else f'{current_orbital_frequency:.4f}'
+        orbital_angular_momentum_unit_vector_string = 'NaN' if current_orbital_angular_momentum_unit_vector is None else f'[{current_orbital_angular_momentum_unit_vector[0]:.4f}, {current_orbital_angular_momentum_unit_vector[1]:.4f}, {current_orbital_angular_momentum_unit_vector[2]:.4f}]'
         ending = f"\nCurrent Values (Last available data):\n" \
                  f"{'-' * 70}\n" \
-                 f"current time:\t\t\t\t{str(current_time)[0:6]}\n" \
-                 f"separation:\t\t\t\t{str(current_separation)[0:6]}\n" \
-                 f"separation unit vector:\t\t\t{[round(i, 4) for i in current_separation_unit_vector]}\n" \
-                 f"orbital frequency:\t\t\t{str(current_orbital_frequency)[0:6]}\n" \
-                 f"orbital angular momentum unit vector:\t{[round(i, 4) for i in current_orbital_angular_momentum_unit_vector]}"
+                 f"current time:\t\t\t\t{time_string}\n" \
+                 f"separation:\t\t\t\t{separation_string}\n" \
+                 f"separation unit vector:\t\t\t{separation_unit_vector_string}\n" \
+                 f"orbital frequency:\t\t\t{orbital_frequency_string}\n" \
+                 f"orbital angular momentum unit vector:\t{orbital_angular_momentum_unit_vector_string}"
     else:
-        ds_message = f"None" if final_dimensionless_spin is None else f"{[round(i, 4) for i in final_dimensionless_spin]}"
+        final_horizon_mass_string = 'NaN' if final_horizon_mass is None else f'{final_horizon_mass:.4f}'
+        final_spin_string = 'NaN' if final_dimensionless_spin is None else f'[{final_dimensionless_spin[0]:.4f}, {final_dimensionless_spin[1]:.4f}, {final_dimensionless_spin[2]:.4f}]'
         ending = f"\nRemnant Values (Last available data):\n" \
                  f"{'-' * 70}\n" \
-                 f"horizon mass:\t\t\t\t{str(final_horizon_mass)[0:6]}\n" \
-                 f"dimensionless spin:\t\t\t{ds_message}"
+                 f"horizon mass:\t\t\t\t{final_horizon_mass_string}\n" \
+                 f"dimensionless spin:\t\t\t{final_spin_string}"
         if final_horizon_mass is None or final_dimensionless_spin is None:
-            ending += "\n" + r"** A 'None' value represents data that has not yet been calculated.**"
+            ending += "\n" + r"** A 'NaN' value represents data that has not yet been calculated.**"
 
     summary = f"{beginning}{middle}{ending}"
 
     # Either print data or write to summary.txt.
     if output_directory is None:
         print(summary)
     else:
```

## Comparing `mayawaves-2023.8.dist-info/METADATA` & `mayawaves-2024.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mayawaves
-Version: 2023.8
+Version: 2024.4
 Summary: A python package for interacting with Einstein Toolkit simulations and the MAYA Catalog of NR Waveforms
 Project-URL: Homepage, https://github.com/MayaWaves/mayawaves
 Project-URL: Bug Tracker, https://github.com/MayaWaves/mayawaves/issues
 Author: Surendra Anne, Miguel Gracia-Linares, Hector Iglesias, Aasim Jan, Erick Martinez, Lu Lu, Filippo Meoni, Ryan Nowicki, Max L. Trostel, Bing-Jyun Tsao, Finny Valorz
 Author-email: Deborah Ferguson <deborah.l.ferguson@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -680,44 +680,28 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Requires-Dist: matplotlib
 Requires-Dist: mock
-Requires-Dist: numba
+Requires-Dist: numba; python_version < '3.11'
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: romspline
 Requires-Dist: scipy
-Requires-Dist: scri
+Requires-Dist: scri; python_version < '3.11'
 Requires-Dist: wget
 Description-Content-Type: text/markdown
 
+[![DOI](https://zenodo.org/badge/685792148.svg)](https://zenodo.org/badge/latestdoi/685792148)
+
 # mayawaves
 
-`Mayawaves` serves as an analysis library for Einstein Toolkit and MAYA simulations. Follow the tutorials to learn how
+`Mayawaves` serves as an analysis library for Einstein Toolkit and MAYA simulations. Follow the tutorials and documentation at https://mayawaves.github.io/mayawaves to learn how
 to use this library to analyze both your own simulations and the simulations in the MAYA Catalog
 (https://cgp.ph.utexas.edu/waveform).
 
-The Coalescence object is the heart of the library. It interacts with an h5 file that contains everything about the
-simulation. Each Coalescence object has CompactObjects for each of the black holes involved in the simulation.
-Refer to the compact_objects tutorial for more details on how to use CompactObjects.
-
-Each Coalescence object also has a RadiationBundle that handles all the information pertaining to gravitational
-radiation. This is primarily done behind the scenes and you can access all gravitational wave information directly
-through Coalescence. Refer to the gravitational_waves tutorial for more information on reading gravitational wave data.
-
-There is also a utility to stitch a raw simulation into the h5 format that the Coalescence object reads. This is
-shown in the creating_h5 tutorial. Coalescence objects can also be exported to the format used by LVK analyses, as shown in
-the exporking_lvk tuttorial.
-
-The catalog_utils tutorial walks through using the Catalog object in the catalogutils module to obtain metadata about
-the MAYA catalog and to download simulations from the MAYA catalog.
-
-## Contributing
 
-`Mayawaves` is intended to be a library that will grow and expand with additional analysis tools. We welcome the 
-input of the community to both request new features and help in implementing them.
```

## Comparing `mayawaves-2023.8.dist-info/licenses/LICENSE` & `mayawaves-2024.4.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

