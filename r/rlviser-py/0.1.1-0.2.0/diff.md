# Comparing `tmp/rlviser_py-0.1.1.tar.gz` & `tmp/rlviser_py-0.2.0.tar.gz`

## Comparing `rlviser_py-0.1.1.tar` & `rlviser_py-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 rlviser_py-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     2774 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/.gitignore
--rw-r--r--   0     1001      123     1070 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/LICENSE
--rw-r--r--   0     1001      123      490 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/README.md
--rw-r--r--   0     1001      123      390 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123      255 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/rlviser_py.pyi
--rw-r--r--   0     1001      123       74 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/rustfmt.toml
--rw-r--r--   0     1001      123    32523 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/src/bytes.rs
--rw-r--r--   0     1001      123      995 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/src/gym.rs
--rw-r--r--   0     1001      123     4209 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123     1351 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/src/socket.rs
--rw-r--r--   0     1001      123     7635 2023-06-06 14:25:07.000000 rlviser_py-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 rlviser_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 rlviser_py-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2774 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     1070 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/LICENSE
+-rw-r--r--   0     1001      123      490 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/README.md
+-rw-r--r--   0     1001      123      390 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      255 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/rlviser_py.pyi
+-rw-r--r--   0     1001      123       74 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/rustfmt.toml
+-rw-r--r--   0     1001      123    32938 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/src/bytes.rs
+-rw-r--r--   0     1001      123      995 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/src/gym.rs
+-rw-r--r--   0     1001      123     4219 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     1351 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/src/socket.rs
+-rw-r--r--   0     1001      123     7635 2023-06-11 06:33:37.000000 rlviser_py-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 rlviser_py-0.2.0/PKG-INFO
```

### Comparing `rlviser_py-0.1.1/Cargo.toml` & `rlviser_py-0.2.0/Cargo.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [package]
 name = "rlviser-py"
-version = "0.1.1"
+version = "0.2.0"
 edition = "2021"
 description = "Python implementation that manages a UDP connection to RLViser"
 license = "MIT"
 repository = "https://github.com/VirxEC/rlviser-py"
 readme = "README.md"
 keywords = ["rlviser", "rocket-league", "udp", "python", "rlbot"]
+publish = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "rlviser_py"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `rlviser_py-0.1.1/.github/workflows/CI.yml` & `rlviser_py-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.1.1/.gitignore` & `rlviser_py-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.1.1/LICENSE` & `rlviser_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.1.1/src/bytes.rs` & `rlviser_py-0.2.0/src/bytes.rs`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     pub is_on_ground: bool,
     pub has_jumped: bool,
     pub has_double_jumped: bool,
     pub has_flipped: bool,
     pub last_rel_dodge_torque: Vec3,
     pub jump_time: f32,
     pub flip_time: f32,
+    pub is_flipping: bool,
     pub is_jumping: bool,
     pub air_time_since_jump: f32,
     pub boost: f32,
     pub time_spent_boosting: f32,
     pub is_supersonic: bool,
     pub supersonic_time: f32,
     pub handbrake_val: f32,
@@ -253,84 +254,89 @@
         // jump_time: f32,
         bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4 + f32::NUM_BYTES]
             .copy_from_slice(&self.jump_time.to_le_bytes());
         // flip_time: f32,
         bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4 + f32::NUM_BYTES
             ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4 + f32::NUM_BYTES * 2]
             .copy_from_slice(&self.flip_time.to_le_bytes());
-        // is_jumping: bool,
+        // is_flipping: bool,
         bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4 + f32::NUM_BYTES * 2
             ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 2]
+            .copy_from_slice(&(self.is_flipping as u8).to_le_bytes());
+        // is_jumping: bool,
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 2
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 2]
             .copy_from_slice(&(self.is_jumping as u8).to_le_bytes());
         // air_time_since_jump: f32,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 2
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 3]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 2
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 3]
             .copy_from_slice(&self.air_time_since_jump.to_le_bytes());
         // boost: f32,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 3
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 4]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 3
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 4]
             .copy_from_slice(&self.boost.to_le_bytes());
         // time_spent_boosting: f32,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 4
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 5]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 4
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 5]
             .copy_from_slice(&self.time_spent_boosting.to_le_bytes());
         // is_supersonic: bool,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 5
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 5]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 5
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 5]
             .copy_from_slice(&(self.is_supersonic as u8).to_le_bytes());
         // supersonic_time: f32,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 5
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 6]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 5
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 6]
             .copy_from_slice(&self.supersonic_time.to_le_bytes());
         // handbrake_val: f32,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 6
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 7]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 6
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 7]
             .copy_from_slice(&self.handbrake_val.to_le_bytes());
         // is_auto_flipping: bool,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 7
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 7]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 7
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 7]
             .copy_from_slice(&(self.is_auto_flipping as u8).to_le_bytes());
         // auto_flip_timer: f32,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 7
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 8]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 7
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 8]
             .copy_from_slice(&self.auto_flip_timer.to_le_bytes());
         // auto_flip_torque_scale: f32,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 8
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 9]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 8
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9]
             .copy_from_slice(&self.auto_flip_torque_scale.to_le_bytes());
         // has_contact: bool,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 9
-            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9
+            ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9]
             .copy_from_slice(&(self.has_contact as u8).to_le_bytes());
         // contact_normal: Vec3,
-        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9
-            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9]
+        bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9
+            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9]
             .copy_from_slice(&self.contact_normal.to_bytes());
         // other_car_id: u32,
-        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9
-            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9 + u32::NUM_BYTES]
+        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9
+            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9 + u32::NUM_BYTES]
             .copy_from_slice(&self.other_car_id.to_le_bytes());
         // cooldown_timer: f32,
-        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9 + u32::NUM_BYTES
-            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 10 + u32::NUM_BYTES]
+        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9 + u32::NUM_BYTES
+            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES]
             .copy_from_slice(&self.cooldown_timer.to_le_bytes());
         // is_demoed: bool,
-        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 10 + u32::NUM_BYTES
-            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES]
+        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES
+            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 10 + u32::NUM_BYTES]
             .copy_from_slice(&(self.is_demoed as u8).to_le_bytes());
         // demo_respawn_timer: f32,
-        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES
-            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 11 + u32::NUM_BYTES]
+        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 10 + u32::NUM_BYTES
+            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 11 + u32::NUM_BYTES]
             .copy_from_slice(&self.demo_respawn_timer.to_le_bytes());
         // ball_hit_info: BallHitInfo,
-        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 11 + u32::NUM_BYTES
-            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 11 + u32::NUM_BYTES + BallHitInfo::NUM_BYTES]
+        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 11 + u32::NUM_BYTES
+            ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 11 + u32::NUM_BYTES + BallHitInfo::NUM_BYTES]
             .copy_from_slice(&self.ball_hit_info.to_bytes());
         // last_controls: CarControls,
-        bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 11 + u32::NUM_BYTES + BallHitInfo::NUM_BYTES..]
+        bytes
+            [Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 11 + u32::NUM_BYTES + BallHitInfo::NUM_BYTES..]
             .copy_from_slice(&self.last_controls.to_bytes());
         bytes
     }
 }
 
 impl ToBytesExact<{ Self::NUM_BYTES }> for CarInfo {
     fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
@@ -533,15 +539,15 @@
         }
     }
 }
 
 impl FromBytesExact for CarState {
     const NUM_BYTES: usize = Vec3::NUM_BYTES * 5
         + RotMat::NUM_BYTES
-        + 9
+        + 10
         + f32::NUM_BYTES * 11
         + u32::NUM_BYTES
         + BallHitInfo::NUM_BYTES
         + CarControls::NUM_BYTES;
 
     #[inline]
     fn from_bytes(bytes: &[u8]) -> Self {
@@ -563,76 +569,77 @@
                 &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4
                     ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4 + f32::NUM_BYTES],
             ),
             flip_time: f32::from_bytes(
                 &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4 + f32::NUM_BYTES
                     ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4 + f32::NUM_BYTES * 2],
             ),
-            is_jumping: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4 + f32::NUM_BYTES * 2] != 0,
+            is_flipping: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 4 + f32::NUM_BYTES * 2] != 0,
+            is_jumping: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 2] != 0,
             air_time_since_jump: f32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 2
-                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 3],
+                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 2
+                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 3],
             ),
             boost: f32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 3
-                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 4],
+                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 3
+                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 4],
             ),
             time_spent_boosting: f32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 4
-                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 5],
+                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 4
+                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 5],
             ),
-            is_supersonic: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 5 + f32::NUM_BYTES * 5] != 0,
+            is_supersonic: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 5] != 0,
             supersonic_time: f32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 5
-                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 6],
+                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 5
+                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 6],
             ),
             handbrake_val: f32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 5
-                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 7],
+                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 5
+                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 7],
             ),
-            is_auto_flipping: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 6 + f32::NUM_BYTES * 7] != 0,
+            is_auto_flipping: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 7] != 0,
             auto_flip_timer: f32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 6
-                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 8],
+                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 6
+                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 8],
             ),
             auto_flip_torque_scale: f32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 7
-                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 9],
+                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 7
+                    ..Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9],
             ),
-            has_contact: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 7 + f32::NUM_BYTES * 9] != 0,
+            has_contact: bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9] != 0,
             contact_normal: Vec3::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 8
-                    ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9],
+                &bytes[Vec3::NUM_BYTES * 4 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 8
+                    ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9],
             ),
             other_car_id: u32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 8
-                    ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 9 + u32::NUM_BYTES],
+                &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 8
+                    ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9 + u32::NUM_BYTES],
             ),
             cooldown_timer: f32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 8 + u32::NUM_BYTES
-                    ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 10 + u32::NUM_BYTES],
+                &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 8 + u32::NUM_BYTES
+                    ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES],
             ),
-            is_demoed: bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 8 + f32::NUM_BYTES * 10 + u32::NUM_BYTES] != 0,
+            is_demoed: bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 10 + u32::NUM_BYTES] != 0,
             demo_respawn_timer: f32::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 9 + u32::NUM_BYTES
-                    ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 11 + u32::NUM_BYTES],
+                &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 9 + u32::NUM_BYTES
+                    ..Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 11 + u32::NUM_BYTES],
             ),
             ball_hit_info: BallHitInfo::from_bytes(
-                &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 9 + f32::NUM_BYTES * 11 + u32::NUM_BYTES
+                &bytes[Vec3::NUM_BYTES * 5 + RotMat::NUM_BYTES + 10 + f32::NUM_BYTES * 11 + u32::NUM_BYTES
                     ..Vec3::NUM_BYTES * 5
                         + RotMat::NUM_BYTES
-                        + 9
+                        + 10
                         + f32::NUM_BYTES * 11
                         + u32::NUM_BYTES
                         + BallHitInfo::NUM_BYTES],
             ),
             last_controls: CarControls::from_bytes(
                 &bytes[Vec3::NUM_BYTES * 5
                     + RotMat::NUM_BYTES
-                    + 9
+                    + 10
                     + f32::NUM_BYTES * 11
                     + u32::NUM_BYTES
                     + BallHitInfo::NUM_BYTES..],
             ),
         }
     }
 }
```

### Comparing `rlviser_py-0.1.1/src/gym.rs` & `rlviser_py-0.2.0/src/gym.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.1.1/src/lib.rs` & `rlviser_py-0.2.0/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 mod socket;
 
 use crate::{
     bytes::{BoostPad, BoostPadState},
     gym::GymState,
 };
 use bytes::{BallState, CarConfig, CarInfo, CarState, GameState, Team, WheelPairConfig};
-use glam::{Mat3A, Quat, Vec3A, EulerRot};
+use glam::{Mat3A, Quat, Vec3A};
 use gym::BOOST_PADS_LENGTH;
 use pyo3::prelude::*;
-use std::{sync::{
+use std::sync::{
     atomic::{AtomicU64, Ordering},
     RwLock,
-}, f32::consts::PI};
+};
 
 macro_rules! pynamedmodule {
     (doc: $doc:literal, name: $name:tt, funcs: [$($func_name:path),*], classes: [$($class_name:ident),*]) => {
         #[doc = $doc]
         #[pymodule]
         #[allow(redundant_semicolons)]
         fn $name(_py: Python, m: &PyModule) -> PyResult<()> {
@@ -67,27 +67,37 @@
         wheel_radius: 15.,
         suspension_rest_length: 37.055,
         connection_point_offset: Vec3A::new(-33.75, 29.5, 20.755),
     },
     dodge_deadzone: 0.5,
 };
 
+#[inline]
+fn ball_to_quat(array: [f32; 4]) -> Quat {
+    Quat::from_xyzw(array[1], array[2], array[3], array[0])
+}
+
+#[inline]
+fn car_to_mat3a(array: [f32; 4]) -> Mat3A {
+    Mat3A::from_quat(Quat::from_xyzw(-array[1], array[2], array[3], array[0]))
+}
+
 /// Reads the RLGym state and sends it to RLViser to render
 #[pyfunction]
 fn render_rlgym(gym_state: GymState) {
     // construct the game state
     let game_state = GameState {
         tick_count: TICK_COUNT.fetch_add(1, Ordering::SeqCst),
         tick_rate: TICK_RATE,
         ball: BallState {
             pos: gym_state.ball.position.into(),
             vel: gym_state.ball.linear_velocity.into(),
             ang_vel: gym_state.ball.angular_velocity.into(),
         },
-        ball_rot: Quat::from_array(gym_state.ball.quaternion),
+        ball_rot: ball_to_quat(gym_state.ball.quaternion),
         pads: BOOST_PAD_LOCATIONS
             .read()
             .unwrap()
             .into_iter()
             .zip(gym_state.boost_pads.into_iter())
             .map(|(position, is_active)| BoostPad {
                 position,
@@ -100,27 +110,21 @@
             .collect(),
         cars: gym_state
             .players
             .into_iter()
             .enumerate()
             .map(|(id, player)| CarInfo {
                 id: id as u32 + 1,
-                team: if player.team_num < 0.5 {
-                    Team::Blue
-                } else {
-                    Team::Orange
-                },
+                team: if player.team_num < 0.5 { Team::Blue } else { Team::Orange },
                 state: CarState {
                     pos: player.car_data.position.into(),
                     vel: player.car_data.linear_velocity.into(),
                     ang_vel: player.car_data.angular_velocity.into(),
-                    rot_mat: {
-                        let (yaw, pitch, roll) = Quat::from_array(player.car_data.quaternion).conjugate().to_euler(EulerRot::ZYX);
-                        Mat3A::from_euler(EulerRot::XYZ, yaw, pitch, roll + PI)
-                    },
+                    rot_mat: car_to_mat3a(player.car_data.quaternion),
+                    is_on_ground: player.on_ground != 0,
                     ..Default::default()
                 },
                 config: OCTANE,
             })
             .collect(),
     };
```

### Comparing `rlviser_py-0.1.1/src/socket.rs` & `rlviser_py-0.2.0/src/socket.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.1.1/Cargo.lock` & `rlviser_py-0.2.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,17 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.0"
@@ -171,15 +171,15 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlviser-py"
-version = "0.1.1"
+version = "0.2.0"
 dependencies = [
  "glam",
  "once_cell",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `rlviser_py-0.1.1/PKG-INFO` & `rlviser_py-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlviser-py
-Version: 0.1.1
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python implementation that manages a UDP connection to RLViser
 Keywords: rlviser,rocket-league,udp,python,rlbot
 License: MIT
```

