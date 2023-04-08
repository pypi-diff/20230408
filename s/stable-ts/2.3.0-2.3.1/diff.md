# Comparing `tmp/stable-ts-2.3.0.tar.gz` & `tmp/stable-ts-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.3.0.tar", last modified: Tue Apr  4 03:55:45 2023, max compression
+gzip compressed data, was "stable-ts-2.3.1.tar", last modified: Sat Apr  8 18:09:49 2023, max compression
```

## Comparing `stable-ts-2.3.0.tar` & `stable-ts-2.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 03:55:45.241386 stable-ts-2.3.0/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.3.0/LICENSE
--rw-rw-rw-   0        0        0     6890 2023-04-04 03:55:45.241386 stable-ts-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-04 03:55:45.241386 stable-ts-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 03:55:45.200386 stable-ts-2.3.0/stable_ts.egg-info/
--rw-rw-rw-   0        0        0     6890 2023-04-04 03:55:44.000000 stable-ts-2.3.0/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-04-04 03:55:45.000000 stable-ts-2.3.0/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 03:55:44.000000 stable-ts-2.3.0/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-04 03:55:44.000000 stable-ts-2.3.0/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-04-04 03:55:44.000000 stable-ts-2.3.0/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-04 03:55:44.000000 stable-ts-2.3.0/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 03:55:45.239386 stable-ts-2.3.0/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.3.0/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.3.0/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-04-04 03:46:30.000000 stable-ts-2.3.0/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     4009 2023-03-25 19:51:29.000000 stable-ts-2.3.0/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4328 2023-03-22 02:57:30.000000 stable-ts-2.3.0/stable_whisper/decode.py
--rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.3.0/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    27563 2023-04-04 03:43:49.000000 stable-ts-2.3.0/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.3.0/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    12410 2023-04-04 03:38:28.000000 stable-ts-2.3.0/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0     9201 2023-03-28 04:22:23.000000 stable-ts-2.3.0/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.3.0/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    48020 2023-04-04 03:43:49.000000 stable-ts-2.3.0/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:09:49.120530 stable-ts-2.3.1/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6890 2023-04-08 18:09:49.119530 stable-ts-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 18:09:49.120530 stable-ts-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:09:49.068530 stable-ts-2.3.1/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0     6890 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-08 18:09:48.000000 stable-ts-2.3.1/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 18:09:49.117530 stable-ts-2.3.1/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.3.1/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.3.1/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-04-08 18:02:41.000000 stable-ts-2.3.1/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     4009 2023-03-25 19:51:29.000000 stable-ts-2.3.1/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4328 2023-03-22 02:57:30.000000 stable-ts-2.3.1/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.3.1/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    27797 2023-04-08 17:41:20.000000 stable-ts-2.3.1/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.3.1/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    12598 2023-04-05 01:42:52.000000 stable-ts-2.3.1/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0     9744 2023-04-08 16:34:45.000000 stable-ts-2.3.1/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.3.1/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    48446 2023-04-08 16:34:45.000000 stable-ts-2.3.1/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.3.0/LICENSE` & `stable-ts-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.0/PKG-INFO` & `stable-ts-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.3.0
+Version: 2.3.1
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.3.0/README.md` & `stable-ts-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.0/setup.py` & `stable-ts-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.0/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.3.1/stable_ts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.3.0
+Version: 2.3.1
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.3.0/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.3.1/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.0/stable_whisper/audio.py` & `stable-ts-2.3.1/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.0/stable_whisper/decode.py` & `stable-ts-2.3.1/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.0/stable_whisper/quantization.py` & `stable-ts-2.3.1/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.0/stable_whisper/result.py` & `stable-ts-2.3.1/stable_whisper/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,16 +327,19 @@
         if not self.has_words or len(self.words) < 2:
             return []
         if isinstance(punctuation, str):
             punctuation = [punctuation]
         indices = []
         for p in punctuation:
             if isinstance(p, str):
-                indices.extend([i for i, w in enumerate(self.words[:-1])
-                                if w.word.endswith(p)])
+                for i, s in enumerate(self.words[:-1]):
+                    if s.word.endswith(p):
+                        indices.append(i)
+                    elif i != 0 and s.word.startswith(p):
+                        indices.append(i-1)
             else:
                 ending, beginning = p
                 indices.extend([i for i, (w0, w1) in enumerate(zip(self.words[:-1], self.words[1:]))
                                 if w0.word.endswith(ending) and w1.word.startswith(beginning)])
 
         return sorted(set(indices) - set(self.get_locked_indices()))
 
@@ -501,16 +504,19 @@
         if len(self.segments) < 2:
             return []
         if isinstance(punctuation, str):
             punctuation = [punctuation]
         indices = []
         for p in punctuation:
             if isinstance(p, str):
-                indices.extend([i for i, s in enumerate(self.segments[:-1])
-                                if s.text.endswith(p)])
+                for i, s in enumerate(self.segments[:-1]):
+                    if s.text.endswith(p):
+                        indices.append(i)
+                    elif i != 0 and s.text.startswith(p):
+                        indices.append(i-1)
             else:
                 ending, beginning = p
                 indices.extend([i for i, (s0, s1) in enumerate(zip(self.segments[:-1], self.segments[1:]))
                                 if s0.text.endswith(ending) and s1.text.startswith(beginning)])
 
         return sorted(set(indices) - set(self.get_locked_indices()))
```

### Comparing `stable-ts-2.3.0/stable_whisper/stabilization.py` & `stable-ts-2.3.1/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.0/stable_whisper/text_output.py` & `stable-ts-2.3.1/stable_whisper/text_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,14 @@
 def segment2assblock(segment: dict, idx: int, strip=True) -> str:
     return f'Dialogue: {idx},{sec2ass(segment["start"])},{sec2ass(segment["end"])},Default,,0,0,0,,' \
            f'{segment["text"].strip() if strip else segment["text"]}'
 
 
 def words2segments(words: List[dict], tag: Tuple[str, str], rtl: bool = False) -> List[dict]:
     def add_tag(idx: int):
-        idx_filled_words = enumerate(filled_words)
-        if rtl:
-            idx_filled_words = reversed(list(idx_filled_words))
         return ''.join(
             (
                 f" {tag[0]}{w['word'][1:]}{tag[1]}"
                 if w['word'].startswith(' ') else
                 f"{tag[0]}{w['word']}{tag[1]}"
             )
             if w['word'] not in ('', ' ') and idx_ == idx else
@@ -79,14 +76,17 @@
     for i, word in enumerate(words):
         curr_end = round(word['end'], 3)
         filled_words.append(dict(word=word['word'], start=round(word['start'], 3), end=curr_end))
         if word != words[-1]:
             next_start = round(words[i + 1]['start'], 3)
             if next_start - curr_end != 0:
                 filled_words.append(dict(word='', start=curr_end, end=next_start))
+    idx_filled_words = list(enumerate(filled_words))
+    if rtl:
+        idx_filled_words = list(reversed(idx_filled_words))
 
     segments = [dict(text=add_tag(i), start=filled_words[i]['start'], end=filled_words[i]['end'])
                 for i in range(len(filled_words))]
     return segments
 
 
 def to_word_level_segments(segments: List[dict], tag: Tuple[str, str]) -> List[dict]:
@@ -148,17 +148,19 @@
         SRT Default: '<font color="#00ff00">', '</font>'
         VTT Default: '<u>', '</u>'
     vtt: bool
         whether to output VTT (default: False if no [filepath] is specified, else determined by [filepath] extension)
     strip: bool
         whether to remove spaces before and after text on each segment for output (default: True)
     rtl: Union[bool, tuple]
-        whether to use Right-To-Left format (default: False)
+        whether to reverse Left-To-Right text into Right-To-Left format (default: False)
         or provide the [prepend_punctuations] and [append_punctuations] as tuple pair instead of True
         to match transcription settings (if True, the default punctuations will be used)
+        Note: This will not fix RTL text not displaying tags properly which is an issue with video player.
+                VLC seems to not suffer from this issue.
 
     Returns
     -------
     string of content if no [filepath] is provided, else None
 
     """
     segments, segment_level, word_level = _preprocess_args(result, segment_level, word_level, min_dur, rtl=rtl)
```

### Comparing `stable-ts-2.3.0/stable_whisper/timing.py` & `stable-ts-2.3.1/stable_whisper/timing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import string
 import torch
 import numpy as np
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, List, Callable
 from itertools import chain
 from whisper.audio import TOKENS_PER_SECOND, N_SAMPLES_PER_TOKEN
 from whisper.timing import WordTiming, median_filter, dtw, merge_punctuations
 
 if TYPE_CHECKING:
     from whisper.tokenizer import Tokenizer
     from whisper.model import Whisper
@@ -141,26 +141,34 @@
 
     return words, word_tokens
 
 
 def split_word_tokens(segments: List[dict],
                       tokenizer: "Tokenizer",
                       *,
-                      padding: (str, int) = None):
+                      padding: (str, int) = None,
+                      split_callback: Callable = None):
     if padding is not None:
         if isinstance(padding, str):
             padding = tokenizer.encode(padding)
         else:
             padding = [padding]
     tokens = []
     seg_indices = []
     words = []
     word_tokens = []
     for i, s in enumerate(segments):
-        curr_words, curr_word_tokens = _split_tokens([t for t in s['tokens'] if t < tokenizer.eot], tokenizer)
+        temp_word_tokens = [t for t in s['tokens'] if t < tokenizer.eot]
+        curr_words, curr_word_tokens = (
+            _split_tokens(temp_word_tokens, tokenizer)
+            if split_callback is None else
+            split_callback(temp_word_tokens, tokenizer)
+        )
+        assert len(curr_words) == len(curr_word_tokens), \
+            f'word count and token group count do not match, {len(curr_words)} and {len(curr_word_tokens)}'
         if (
                 padding is not None and
                 curr_word_tokens[0][0] != padding and
                 (len(tokens) == 0 or tokens[-1] != padding)
         ):
             tokens.extend(padding)
             words.append(None)
@@ -187,14 +195,15 @@
         num_samples: int,
         prepend_punctuations: str = "\"'“¿([{-",
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         audio_features: torch.Tensor = None,
         ts_num: int = 0,
         ts_noise: float = 0.1,
         min_word_dur: float = 0.1,
+        split_callback: Callable = None,
         **kwargs,
 ):
     if len(segments) == 0:
         return
 
     if min_word_dur is None:
         min_word_dur = 0
@@ -204,15 +213,16 @@
 
     if prepend_punctuations is None:
         prepend_punctuations = "\"'“¿([{-"
 
     if append_punctuations is None:
         append_punctuations = "\"'.。,，!！?？:：”)]}、"
 
-    text_tokens, token_split, seg_indices = split_word_tokens(segments, tokenizer, padding=' ...')
+    text_tokens, token_split, seg_indices = split_word_tokens(segments, tokenizer,
+                                                              padding=' ...', split_callback=split_callback)
 
     alignment = find_alignment_stable(model, tokenizer, text_tokens, mel, num_samples,
                                       **kwargs,
                                       token_split=token_split,
                                       audio_features=audio_features,
                                       ts_num=ts_num,
                                       ts_noise=ts_noise)
```

### Comparing `stable-ts-2.3.0/stable_whisper/video_output.py` & `stable-ts-2.3.1/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.3.0/stable_whisper/whisper_word_level.py` & `stable-ts-2.3.1/stable_whisper/whisper_word_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import warnings
 import torch
 import numpy as np
-from typing import TYPE_CHECKING, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, List, Optional, Tuple, Union, Callable
 from types import MethodType
 from tqdm import tqdm
 
 import whisper
 from whisper.audio import (
     SAMPLE_RATE, N_FRAMES, HOP_LENGTH, N_SAMPLES, N_SAMPLES_PER_TOKEN, TOKENS_PER_SECOND, FRAMES_PER_SECOND, N_FFT,
     pad_or_trim, log_mel_spectrogram
@@ -56,14 +56,15 @@
         vad_threshold: float = 0.35,
         vad_onnx: bool = False,
         min_word_dur: float = 0.1,
         only_voice_freq: bool = False,
         prepend_punctuations: str = "\"'“¿([{-",
         append_punctuations: str = "\"'.。,，!！?？:：”)]}、",
         mel_first: bool = False,
+        split_callback: Callable = None,
         **decode_options) \
         -> WhisperResult:
     """
     Transcribe an audio file using Whisper
 
     Parameters
     ----------
@@ -169,14 +170,19 @@
     append_punctuations: str
         Punctuations to append to previous word (Default: .。,，!！?？:：”)]}、)
 
     mel_first: bool
         Process entire audio track into log-Mel spectrogram first instead in chunks. (Default: False)
         Used if odd behavior seen in stable-ts but not in whisper, but use significantly more memory for long audio.
 
+    split_callback: Callable
+        Custom callback for grouping tokens up with their corresponding words.
+        Takes argument: list of tokens; default tokenizer
+        Returns a tuple pair containing: list of words; list of token groups (i.e. each group is list of token(s))
+
     decode_options: dict
         Keyword arguments to construct `DecodingOptions` instances
 
     Returns
     -------
     A dictionary containing the resulting text ("text") and segment-level details ("segments"), and
     the spoken language ("language"), which is detected when `decode_options["language"]` is None.
@@ -228,15 +234,15 @@
             from torchaudio.functional import resample
             if isinstance(audio, np.ndarray):
                 audio = torch.from_numpy(audio)
             audio = resample(audio, input_sr, curr_sr, resampling_method="kaiser_window")
     if only_voice_freq:
         from .audio import voice_freq_filter
         audio = voice_freq_filter(audio, curr_sr)
-    sample_padding = int(N_FFT//2)+1
+    sample_padding = int(N_FFT // 2) + 1
     whole_mel = log_mel_spectrogram(audio, padding=sample_padding) if mel_first else None
 
     if decode_options.get("language", None) is None:
         if verbose:
             print("Detecting language using up to the first 30 seconds. Use `--language` to specify the language")
         mel_segment = log_mel_spectrogram(audio[..., :N_SAMPLES], padding=sample_padding) \
             if whole_mel is None else whole_mel[..., :N_FRAMES]
@@ -326,15 +332,15 @@
             "avg_logprob": result.avg_logprob,
             "compression_ratio": result.compression_ratio,
             "no_speech_prob": result.no_speech_prob,
         }
 
     total_samples = audio.shape[-1]
     total_duration = round(total_samples / curr_sr, 2)
-    n_samples_per_frame = exact_div(N_SAMPLES_PER_TOKEN * TOKENS_PER_SECOND,  FRAMES_PER_SECOND)
+    n_samples_per_frame = exact_div(N_SAMPLES_PER_TOKEN * TOKENS_PER_SECOND, FRAMES_PER_SECOND)
 
     silence_timing = None
     if suppress_silence and vad:
         silence_timing = get_vad_silence_func(onnx=vad_onnx, verbose=verbose)(audio, speech_threshold=vad_threshold)
 
     with tqdm(total=total_duration, unit='sec', disable=verbose is not False) as tqdm_pbar:
 
@@ -359,15 +365,15 @@
             time_offset = seek_sample / SAMPLE_RATE
             segment_samples = min(N_SAMPLES, total_samples - seek_sample)
             segment_duration = segment_samples / SAMPLE_RATE
 
             mel_segment = (
                 log_mel_spectrogram(audio_segment, padding=sample_padding)
                 if whole_mel is None else
-                whole_mel[..., round(seek_sample/n_samples_per_frame): round(seek_sample_end/n_samples_per_frame)]
+                whole_mel[..., round(seek_sample / n_samples_per_frame): round(seek_sample_end / n_samples_per_frame)]
             )
 
             mel_segment = pad_or_trim(mel_segment, N_FRAMES).to(device=model.device, dtype=dtype)
 
             segment_silence_timing = None
             ts_token_mask = None
             if suppress_silence:
@@ -488,15 +494,16 @@
                     tokenizer=tokenizer,
                     mel=mel_segment,
                     num_samples=segment_samples,
                     prepend_punctuations=prepend_punctuations,
                     append_punctuations=append_punctuations,
                     audio_features=audio_features,
                     ts_num=ts_num,
-                    ts_noise=ts_noise
+                    ts_noise=ts_noise,
+                    split_callback=split_callback
                 )
 
             if segment_silence_timing is not None:
                 for seg_i, segment in enumerate(current_segments):
                     current_segments[seg_i] = (
                         Segment(**segment)
                         .suppress_silence(
@@ -746,15 +753,15 @@
                              "ASS Default: '{\\1c&HFF00&}', '{\\r}'")
     parser.add_argument('--segment_level', type=str2bool, default=True,
                         help="whether to use segment-level timestamps in output")
     parser.add_argument('--word_level', type=str2bool, default=True,
                         help="whether to use word-level timestamps in output")
 
     parser.add_argument('--rtl', type=str2bool, default=False,
-                        help="whether to use Right-To-Left format for text outputs")
+                        help="whether to reverse Left-To-Right text into Right-To-Left format for text outputs")
 
     # ass output
     parser.add_argument('--font', type=str, default='Arial',
                         help="word font for ASS output(s)")
     parser.add_argument('--font_size', type=int, default=48,
                         help="word font size for ASS output(s)")
```

