# Comparing `tmp/fir1-1.7.1.1.tar.gz` & `tmp/fir1-1.8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fir1-1.7.1.1.tar", last modified: Wed Nov  3 21:57:49 2021, max compression
+gzip compressed data, was "fir1-1.8.0.0.tar", last modified: Mon Apr 15 13:27:06 2024, max compression
```

## Comparing `fir1-1.7.1.1.tar` & `fir1-1.8.0.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 bp1       (1000) bp1       (1000)        0 2021-11-03 21:57:49.446088 fir1-1.7.1.1/
--rw-rw-r--   0 bp1       (1000) bp1       (1000)     3192 2021-10-17 13:00:45.000000 fir1-1.7.1.1/Fir1.cpp
--rw-rw-r--   0 bp1       (1000) bp1       (1000)     6011 2021-10-17 13:00:45.000000 fir1-1.7.1.1/Fir1.h
--rw-r--r--   0 bp1       (1000) bp1       (1000)       83 2021-11-03 21:56:58.000000 fir1-1.7.1.1/MANIFEST.in
--rw-rw-r--   0 bp1       (1000) bp1       (1000)     3654 2021-11-03 21:57:49.446088 fir1-1.7.1.1/PKG-INFO
--rw-rw-r--   0 bp1       (1000) bp1       (1000)     9062 2021-10-31 01:01:00.000000 fir1-1.7.1.1/README.md
--rw-rw-r--   0 bp1       (1000) bp1       (1000)     2494 2021-09-18 11:50:01.000000 fir1-1.7.1.1/README_py.rst
-drwxrwxr-x   0 bp1       (1000) bp1       (1000)        0 2021-11-03 21:57:49.446088 fir1-1.7.1.1/fir1.egg-info/
--rw-r--r--   0 bp1       (1000) bp1       (1000)     3654 2021-11-03 21:57:49.000000 fir1-1.7.1.1/fir1.egg-info/PKG-INFO
--rw-r--r--   0 bp1       (1000) bp1       (1000)      222 2021-11-03 21:57:49.000000 fir1-1.7.1.1/fir1.egg-info/SOURCES.txt
--rw-r--r--   0 bp1       (1000) bp1       (1000)        1 2021-11-03 21:57:49.000000 fir1-1.7.1.1/fir1.egg-info/dependency_links.txt
--rw-r--r--   0 bp1       (1000) bp1       (1000)        6 2021-11-03 21:57:49.000000 fir1-1.7.1.1/fir1.egg-info/requires.txt
--rw-r--r--   0 bp1       (1000) bp1       (1000)       11 2021-11-03 21:57:49.000000 fir1-1.7.1.1/fir1.egg-info/top_level.txt
--rw-rw-r--   0 bp1       (1000) bp1       (1000)     1406 2021-09-17 08:22:31.000000 fir1-1.7.1.1/fir1.i
--rw-rw-r--   0 bp1       (1000) bp1       (1000)     3540 2021-11-03 21:43:04.000000 fir1-1.7.1.1/fir1.py
--rw-r--r--   0 bp1       (1000) bp1       (1000)   107369 2018-11-06 14:03:49.000000 fir1-1.7.1.1/numpy.i
--rw-rw-r--   0 bp1       (1000) bp1       (1000)       38 2021-11-03 21:57:49.446088 fir1-1.7.1.1/setup.cfg
--rwxrwxr-x   0 bp1       (1000) bp1       (1000)     1486 2021-11-03 21:57:17.000000 fir1-1.7.1.1/setup.py
+drwxrwxr-x   0 bp1       (1000) bp1       (1000)        0 2024-04-15 13:27:06.319928 fir1-1.8.0.0/
+-rw-r--r--   0 bp1       (1000) bp1       (1000)       25 2020-03-06 09:42:22.000000 fir1-1.8.0.0/AUTHORS
+-rw-r--r--   0 bp1       (1000) bp1       (1000)     1140 2020-03-06 09:42:22.000000 fir1-1.8.0.0/COPYING
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     3579 2024-04-15 12:22:16.000000 fir1-1.8.0.0/Fir1.cpp
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     6703 2024-04-15 12:36:58.000000 fir1-1.8.0.0/Fir1.h
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)       83 2021-11-05 16:02:53.000000 fir1-1.8.0.0/MANIFEST.in
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     2941 2024-04-15 13:27:06.319928 fir1-1.8.0.0/PKG-INFO
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     8280 2024-04-15 12:46:56.000000 fir1-1.8.0.0/README.md
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     2492 2024-04-15 13:02:20.000000 fir1-1.8.0.0/README_py.rst
+drwxrwxr-x   0 bp1       (1000) bp1       (1000)        0 2024-04-15 13:27:06.319928 fir1-1.8.0.0/fir1.egg-info/
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     2941 2024-04-15 13:27:06.000000 fir1-1.8.0.0/fir1.egg-info/PKG-INFO
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)      238 2024-04-15 13:27:06.000000 fir1-1.8.0.0/fir1.egg-info/SOURCES.txt
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)        1 2024-04-15 13:27:06.000000 fir1-1.8.0.0/fir1.egg-info/dependency_links.txt
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)        6 2024-04-15 13:27:06.000000 fir1-1.8.0.0/fir1.egg-info/requires.txt
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)       11 2024-04-15 13:27:06.000000 fir1-1.8.0.0/fir1.egg-info/top_level.txt
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     1418 2024-04-15 13:20:59.000000 fir1-1.8.0.0/fir1.i
+-rw-r--r--   0 bp1       (1000) bp1       (1000)     3712 2024-04-15 13:21:47.000000 fir1-1.8.0.0/fir1.py
+-rw-r--r--   0 bp1       (1000) bp1       (1000)   107369 2020-03-06 09:42:22.000000 fir1-1.8.0.0/numpy.i
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)       38 2024-04-15 13:27:06.319928 fir1-1.8.0.0/setup.cfg
+-rwxrwxr-x   0 bp1       (1000) bp1       (1000)     1486 2024-04-15 13:15:58.000000 fir1-1.8.0.0/setup.py
```

### Comparing `fir1-1.7.1.1/Fir1.cpp` & `fir1-1.8.0.0/Fir1.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -17,41 +17,43 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 */
 
 /* (C) 2013 Graeme Hattan & Bernd Porr */
-/* (C) 2018-2021 Bernd Porr */
+/* (C) 2018-2024 Bernd Porr */
 
 #include "Fir1.h"
 
 #include <string.h>
 #include <stdlib.h>
 #include <assert.h>
 #include <stdexcept>
 
 // give the filter an array of doubles for the coefficients
-Fir1::Fir1(double *_coefficients, unsigned number_of_taps) :
+Fir1::Fir1(const double *_coefficients,const unsigned number_of_taps) :
 	coefficients(new double[number_of_taps]),
 	buffer(new double[number_of_taps]()),
 	taps(number_of_taps) {
 	for(unsigned int i=0;i<number_of_taps;i++) {
 		coefficients[i] = _coefficients[i];
 		buffer[i] = 0;
 	}
 }
 
 // init all coefficients and the buffer to zero
-Fir1::Fir1(unsigned number_of_taps) :
+Fir1::Fir1(unsigned number_of_taps, double value) :
 	coefficients(new double[number_of_taps]),
 	buffer(new double[number_of_taps]),  
 	taps(number_of_taps) {
-	zeroCoeff();
-	reset();
+	for(unsigned int i=0;i<number_of_taps;i++) {
+	        coefficients[i] = value;
+		buffer[i] = 0;
+	}
 }
 
 void Fir1::initWithVector(std::vector<double> _coefficients) {
 	coefficients = new double[_coefficients.size()];
 	buffer = new double[_coefficients.size()]();
 	taps = ((unsigned int)_coefficients.size());
 	for(unsigned long i=0;i<_coefficients.size();i++) {
@@ -103,8 +105,17 @@
 	if (number_of_taps < taps)
 		throw std::out_of_range("Fir1: target of getCoeff: too many weights to copy into target");
  
 	memcpy(coeff_data, coefficients, taps * sizeof(double));
 	if (number_of_taps > taps)
 		memset(&coeff_data[taps], 0, (number_of_taps - taps)*sizeof(double));
 }
+void Fir1::setCoeff(const double* coeff_data, const unsigned number_of_taps) {
+
+	if (number_of_taps != taps) {
+		throw std::runtime_error("Invalid number of taps in new coefficient array");
+	}
+	for (unsigned int i = 0; i < number_of_taps; i++) {
+		coefficients[i] = coeff_data[i];
+	}
+}
```

### Comparing `fir1-1.7.1.1/Fir1.h` & `fir1-1.8.0.0/Fir1.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,212 +1,225 @@
 /*
-License: MIT License (http://www.opensource.org/licenses/mit-license.php)
+  License: MIT License (http://www.opensource.org/licenses/mit-license.php)
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+  Permission is hereby granted, free of charge, to any person obtaining a copy
+  of this software and associated documentation files (the "Software"), to deal
+  in the Software without restriction, including without limitation the rights
+  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+  copies of the Software, and to permit persons to whom the Software is
+  furnished to do so, subject to the following conditions:
+
+  The above copyright notice and this permission notice shall be included in
+  all copies or substantial portions of the Software.
+
+  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+  THE SOFTWARE.
 */
 
-/* (C) 2013-2021 Graeme Hattan & Bernd Porr */
+/* (C) 2013-2024 Graeme Hattan & Bernd Porr */
 
 #ifndef FIR1_H
 #define FIR1_H
 
 #include <stdio.h>
 #include <vector>
 
 /**
  * Finite impulse response filter. The precision is double.
  * It takes as an input a file with coefficients or an double
  * array.
  **/
 class Fir1 {
 public:
-	/** 
-         * Coefficients as a const double array. Because the array is const
-         * the number of taps is identical to the length of the array.
-         * \param _coefficients A const double array with the impulse response.
-         **/
-	template <unsigned nTaps> Fir1(const double (&_coefficients)[nTaps]) :
-		coefficients(new double[nTaps]),
-		buffer(new double[nTaps]()),
-		taps(nTaps) {
-		for(unsigned i=0;i<nTaps;i++) {
-			coefficients[i] = _coefficients[i];
-			buffer[i] = 0;
-		}
-	}
-
-	/**
-	 * Coefficients as a C++ vector
-	 * \param _coefficients is a Vector of doubles.
-	 **/
-	Fir1(std::vector<double> _coefficients) {
-		initWithVector(_coefficients);
-	}
-
-	/**
-         * Coefficients as a (non-constant-) double array where the length needs to be specified.
-	 * \param coefficients Coefficients as double array.
-         * \param number_of_taps Number of taps (needs to match the number of coefficients
-         **/
-	Fir1(double *coefficients, unsigned number_of_taps);
-
-	/** Coefficients as a text file (for example from Python)
-	 * The number of taps is automatically detected
-	 * when the taps are kept zero.
-         * \param coeffFile Patht to textfile where every line contains one coefficient
-         * \param number_of_taps Number of taps (0 = autodetect)
-         **/
-	Fir1(const char* coeffFile, unsigned number_of_taps = 0);
-
-	/** 
-         * Inits all coefficients and the buffer to zero
-	 * This is useful for adaptive filters where we start with
-	 * zero valued coefficients.
-         **/
-	Fir1(unsigned number_of_taps);
-
-	/**
-         * Releases the coefficients and buffer.
-         **/
-	~Fir1();
+    /** 
+     * Coefficients as a const double array. Because the array is const
+     * the number of taps is identical to the length of the array.
+     * \param _coefficients A const double array with the impulse response.
+     **/
+    template <unsigned nTaps> Fir1(const double (&_coefficients)[nTaps]) :
+	coefficients(new double[nTaps]),
+	buffer(new double[nTaps]()),
+	taps(nTaps) {
+	for(unsigned i=0;i<nTaps;i++) {
+	    coefficients[i] = _coefficients[i];
+	    buffer[i] = 0;
+	}
+    }
+
+    /**
+     * Coefficients as a C++ vector
+     * \param _coefficients is a Vector of doubles.
+     **/
+    Fir1(std::vector<double> _coefficients) {
+	initWithVector(_coefficients);
+    }
+
+    /**
+     * Coefficients as a (non-constant-) double array where the length needs to be specified.
+     * \param coefficients Coefficients as double array.
+     * \param number_of_taps Number of taps (needs to match the number of coefficients
+     **/
+    Fir1(const double *coefficients,const unsigned number_of_taps);
+
+    /** Coefficients as a text file (for example from Python)
+     * The number of taps is automatically detected
+     * when the taps are kept zero.
+     * \param coeffFile Patht to textfile where every line contains one coefficient
+     * \param number_of_taps Number of taps (0 = autodetect)
+     **/
+    Fir1(const char* coeffFile, unsigned number_of_taps = 0);
+
+    /** 
+     * Inits all coefficients and the buffer to a constant value.
+     * This is useful for adaptive filters where we start with
+     * zero valued coefficients or moving average filters with
+     * value = 1.0/number_of_taps.
+     **/
+    Fir1(unsigned number_of_taps, double value = 0);
+
+    /**
+     * Releases the coefficients and buffer.
+     **/
+    ~Fir1();
 
 	
-	/**
-         * The actual filter function operation: it receives one sample
-         * and returns one sample.
-         * \param input The input sample.
-         **/
-	inline double filter(double input) {
-		const double *coeff     = coefficients;
-		const double *const coeff_end = coefficients + taps;
-		
-		double *buf_val = buffer + offset;
-		
-		*buf_val = input;
-		double output_ = 0;
-		
-		while(buf_val >= buffer)
-			output_ += *buf_val-- * *coeff++;
-		
-		buf_val = buffer + taps-1;
-		
-		while(coeff < coeff_end)
-			output_ += *buf_val-- * *coeff++;
-		
-		if(++offset >= taps)
-			offset = 0;
-		
-		return output_;
-	}
-
-
-	/**
-         * LMS adaptive filter weight update:
-	 * Every filter coefficient is updated with:
-	 * w_k(n+1) = w_k(n) + learning_rate * buffer_k(n) * error(n)
-         * \param error Is the term error(n), the error which adjusts the FIR conefficients.
-         **/
-	inline void lms_update(double error) {
-		double *coeff     = coefficients;
-		const double *coeff_end = coefficients + taps;
+    /**
+     * The actual filter function operation: it receives one sample
+     * and returns one sample.
+     * \param input The input sample.
+     **/
+    inline double filter(double input) {
+	const double *coeff     = coefficients;
+	const double *const coeff_end = coefficients + taps;
+		
+	double *buf_val = buffer + offset;
+		
+	*buf_val = input;
+	double output_ = 0;
+		
+	while(buf_val >= buffer)
+	    output_ += *buf_val-- * *coeff++;
+		
+	buf_val = buffer + taps-1;
+		
+	while(coeff < coeff_end)
+	    output_ += *buf_val-- * *coeff++;
+		
+	if(++offset >= taps)
+	    offset = 0;
+		
+	return output_;
+    }
+
+
+    /**
+     * LMS adaptive filter weight update:
+     * Every filter coefficient is updated with:
+     * w_k(n+1) = w_k(n) + learning_rate * buffer_k(n) * error(n)
+     * \param error Is the term error(n), the error which adjusts the FIR conefficients.
+     **/
+    inline void lms_update(double error) {
+	double *coeff     = coefficients;
+	const double *coeff_end = coefficients + taps;
 	
-		double *buf_val = buffer + offset;
+	double *buf_val = buffer + offset;
 		
-		while(buf_val >= buffer) {
-			*coeff++ += *buf_val-- * error * mu;
-		}
+	while(buf_val >= buffer) {
+	    *coeff++ += *buf_val-- * error * mu;
+	}
 		
-		buf_val = buffer + taps-1;
+	buf_val = buffer + taps-1;
 		
-		while(coeff < coeff_end) {
-			*coeff++ += *buf_val-- * error * mu;
-		}
+	while(coeff < coeff_end) {
+	    *coeff++ += *buf_val-- * error * mu;
+	}
+    }
+
+    /**
+     * Setting the learning rate for the adaptive filter.
+     * \param _mu The learning rate (i.e. rate of the change by the error signal)
+     **/
+    void setLearningRate(double _mu) {mu = _mu;};
+
+    /**
+     * Getting the learning rate for the adaptive filter.
+     **/
+    double getLearningRate() {return mu;};
+
+    /**
+     * Resets the buffer (but not the coefficients)
+     **/
+    void reset();
+
+    /** 
+     * Sets all coefficients to zero
+     **/
+    void zeroCoeff();
+
+    /**
+     * Copies the current filter coefficients into a provided array.
+     * Useful after an adaptive filter has been trained to query
+     * the result of its training.
+     * \param coeff_data target where coefficients are copied
+     * \param number_of_taps number of doubles to be copied
+     * \throws std::out_of_range number_of_taps is less the actual number of taps.
+     */
+    void getCoeff(double* coeff_data, unsigned number_of_taps) const;
+
+    /**
+     * @brief Externally sets the coefficient array. This is useful when the
+     * actually running filter is at a different place as where the updating
+     * filter is employed.
+     *
+     * @param coeff_data New coefficients to set.
+     * @param number_of_taps Number of taps in the coefficient array. If this is
+     * not equal to the number of taps used in this filter, a runtime error is
+     * thrown.
+     */
+    void setCoeff(const double *coeff_data, const unsigned number_of_taps);
+
+    /**
+     * Returns the coefficients as a vector
+     **/
+    std::vector<double> getCoeffVector() const {
+	return std::vector<double>(coefficients,coefficients+taps);
+    }
+
+    /**
+     * Returns the number of taps.
+     **/
+    unsigned getTaps() {return taps;};
+
+    /**
+     * Returns the power of the of the buffer content:
+     * sum_k buffer[k]^2
+     * which is needed to implement a normalised LMS algorithm.
+     **/
+    inline double getTapInputPower() {
+	double *buf_val = buffer;
+		
+	double p = 0;
+		
+	for(unsigned i = 0; i < taps; i++) {
+	    p += (*buf_val) * (*buf_val);
+	    buf_val++;
 	}
-
-	/**
-         * Setting the learning rate for the adaptive filter.
-         * \param _mu The learning rate (i.e. rate of the change by the error signal)
-         **/
-	void setLearningRate(double _mu) {mu = _mu;};
-
-	/**
-         * Getting the learning rate for the adaptive filter.
-         **/
-	double getLearningRate() {return mu;};
-
-	/**
-         * Resets the buffer (but not the coefficients)
-         **/
-	void reset();
-
-	/** 
-         * Sets all coefficients to zero
-         **/
-	void zeroCoeff();
-
-	/**
-	 * Copies the current filter coefficients into a provided array.
-	 * Useful after an adaptive filter has been trained to query
-	 * the result of its training.
-	 * \param coeff_data target where coefficients are copied
-	 * \param number_of_taps number of doubles to be copied
-	 * \throws std::out_of_range number_of_taps is less the actual number of taps.
-	 */
-	void getCoeff(double* coeff_data, unsigned number_of_taps) const;
-
-	/**
-	 * Returns the coefficients as a vector
-	 **/
-	std::vector<double> getCoeffVector() const {
-		return std::vector<double>(coefficients,coefficients+taps);
-	}
-
-	/**
-         * Returns the number of taps.
-         **/
-	unsigned getTaps() {return taps;};
-
-	/**
-         * Returns the power of the of the buffer content:
-	 * sum_k buffer[k]^2
-	 * which is needed to implement a normalised LMS algorithm.
-         **/
-	inline double getTapInputPower() {
-		double *buf_val = buffer;
-		
-		double p = 0;
-		
-		for(unsigned i = 0; i < taps; i++) {
-			p += (*buf_val) * (*buf_val);
-			buf_val++;
-		}
 	
-		return p;
-	}
+	return p;
+    }
 
 private:
-	void initWithVector(std::vector<double> _coefficients);
+    void initWithVector(std::vector<double> _coefficients);
 	
-	double        *coefficients;
-	double        *buffer;
-	unsigned      taps;
-	unsigned      offset = 0;
-	double        mu = 0;
+    double        *coefficients;
+    double        *buffer;
+    unsigned      taps;
+    unsigned      offset = 0;
+    double        mu = 0;
 };
 
 #endif
```

### Comparing `fir1-1.7.1.1/PKG-INFO` & `fir1-1.8.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,111 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fir1
-Version: 1.7.1.1
+Version: 1.8.0.0
 Summary: Efficient FIR realtime filter
 Home-page: https://github.com/berndporr/fir1
 Author: Bernd Porr
 Author-email: mail@berndporr.me.uk
 License: MIT
-Description: ====
-        Fir1
-        ====
-        
-        An efficient Finite Impulse Response (FIR) filter class
-        written in C++ with python wrapper.
-        
-        Adaptive filtering is also implemented using the Least Mean 
-        Square (LMS) or Normalised Least Mean
-        Square (NLMS) algorithm.
-        
-        Installation
-        ============
-        
-        Install the python package with pip::
-        
-            pip3 install fir1
-        
-        You can also install from source::
-        
-            git clone https://github.com/berndporr/fir1
-            cd fir1
-            python3 setup.py install
-        
-        
-        Usage
-        =====
-        
-        Realtime filtering
-        ------------------
-        
-        The filter is a realtime filter which receives samples
-        one by one so it can process data as it arrives from
-        an ADC converter. This is simulated here with the for loop::
-        
-            import fir1
-            b = signal.firwin(999,0.1)
-            f = fir1.Fir1(b)
-            for i in range(len(noisy_signal)):
-                clean_signal[i] = f.filter(noisy_signal[i])
-        
-        The constructor ``Fir1()`` receives the filter coefficients 
-        (= impulse response) and then filtering is performed 
-        with the method ``filter()``.
-        
-        
-        LMS adaptive filter
-        -------------------
-        
-        The file `lms_50Hz_ecg_filter.py` removes 50Hz from 
-        an ECG with the help of the lms filter. 
-        The filter learns its own frequency response from a
-        reference 50Hz sine wave::
-        
-            f = fir1.Fir1(NTAPS)
-            f.setLearningRate(LEARNING_RATE);
-        
-            y= np.empty(len(ecg))
-            for i in range(len(ecg)):
-                ref_noise = np.sin(2.0 * np.pi / 20.0 * i);
-                canceller = f.filter(ref_noise)
-                output_signal = ecg[i] - canceller
-                f.lms_update(output_signal)
-                y[i] = output_signal
-        
-        You can query the filter coefficients using getCoeff.
-        This is most useful to obtain the kernel of a trained
-        adaptive filter::
-        
-                >>> from fir1 import Fir1
-                >>> fir = Fir1([.25, -.5, 1, -.5, .25])
-                >>> fir.getCoeff()
-                array([ 0.25, -0.5 ,  1.  , -0.5 ,  0.25])
-        
-        You may override the length of array to return and
-        the result will be zero-padded. Specifying too small an array
-        causes an exception to be raised::
-        
-                >>> fir.getCoeff(8)
-                array([ 0.25, -0.5 ,  1.  , -0.5 ,  0.25,  0.  ,  0.  ,  0.  ])
-                >>> fir.getCoeff(3)
-                Traceback (most recent call last):
-                File "<stdin>", line 1, in <module>
-                File ".../fir1.py", line 97, in getCoeff
-                return _fir1.Fir1_getCoeff(self, *args)
-                RuntimeError: Fir1: target of getCoeff: too many weights to copy into target
-        
-        
-        Both the demo file and an explanation how the LMS
-        filter works can be found on the homepage of the
-        project:
-        
-        https://github.com/berndporr/fir1
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
+License-File: COPYING
+License-File: AUTHORS
+
+====
+Fir1
+====
+
+An efficient Finite Impulse Response (FIR) filter class
+written in C++ with python wrapper.
+
+Adaptive filtering is also implemented using the Least Mean 
+Square (LMS) or Normalised Least Mean
+Square (NLMS) algorithm.
+
+Installation
+============
+
+Install the python package with pip::
+
+    pip install fir1
+
+You can also install from source::
+
+    git clone https://github.com/berndporr/fir1
+    cd fir1
+    python setup.py install
+
+
+Usage
+=====
+
+Realtime filtering
+------------------
+
+The filter is a realtime filter which receives samples
+one by one so it can process data as it arrives from
+an ADC converter. This is simulated here with the for loop::
+
+    import fir1
+    b = signal.firwin(999,0.1)
+    f = fir1.Fir1(b)
+    for i in range(len(noisy_signal)):
+        clean_signal[i] = f.filter(noisy_signal[i])
+
+The constructor ``Fir1()`` receives the filter coefficients 
+(= impulse response) and then filtering is performed 
+with the method ``filter()``.
+
+
+LMS adaptive filter
+-------------------
+
+The file `lms_50Hz_ecg_filter.py` removes 50Hz from 
+an ECG with the help of the lms filter. 
+The filter learns its own frequency response from a
+reference 50Hz sine wave::
+
+    f = fir1.Fir1(NTAPS)
+    f.setLearningRate(LEARNING_RATE);
+
+    y= np.empty(len(ecg))
+    for i in range(len(ecg)):
+        ref_noise = np.sin(2.0 * np.pi / 20.0 * i);
+        canceller = f.filter(ref_noise)
+        output_signal = ecg[i] - canceller
+        f.lms_update(output_signal)
+        y[i] = output_signal
+
+You can query the filter coefficients using getCoeff.
+This is most useful to obtain the kernel of a trained
+adaptive filter::
+
+        >>> from fir1 import Fir1
+        >>> fir = Fir1([.25, -.5, 1, -.5, .25])
+        >>> fir.getCoeff()
+        array([ 0.25, -0.5 ,  1.  , -0.5 ,  0.25])
+
+You may override the length of array to return and
+the result will be zero-padded. Specifying too small an array
+causes an exception to be raised::
+
+        >>> fir.getCoeff(8)
+        array([ 0.25, -0.5 ,  1.  , -0.5 ,  0.25,  0.  ,  0.  ,  0.  ])
+        >>> fir.getCoeff(3)
+        Traceback (most recent call last):
+        File "<stdin>", line 1, in <module>
+        File ".../fir1.py", line 97, in getCoeff
+        return _fir1.Fir1_getCoeff(self, *args)
+        RuntimeError: Fir1: target of getCoeff: too many weights to copy into target
+
+
+Both the demo file and an explanation how the LMS
+filter works can be found on the homepage of the
+project:
+
+https://github.com/berndporr/fir1
+
+
```

### Comparing `fir1-1.7.1.1/README.md` & `fir1-1.8.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,45 +8,27 @@
 The floating point class offers also adaptive filtering
 using the least mean square (LMS) or normalised least mean
 square (NLMS) algorithm.
 
 
 ## Installation
 
-### Ubuntu packages for xenial, bionic and focal
+### Packages for Ubuntu LTS
 
 Add this repository to your package manager:
 ```
 sudo add-apt-repository ppa:berndporr/dsp
 sudo apt-get update
 sudo apt install fir1
 sudo apt install fir1-dev
 ```
 This adds `fir1-dev` and `fir1` to your package list.
 The demo files are in `/usr/share/doc/fir1-dev`. Copy them into a working
 directory, type `gunzip *.gz`, `cmake .` and `make`.
 
-### MacOS packages (homebrew)
-
-Make sure you have the homebrew package manager installed: https://brew.sh/
-
-Add the homebrew tap:
-
-```
-brew tap berndporr/dsp
-```
-
-and then install the fir filter package with:
-
-```
-brew install fir
-```
-
-
-
 ### Linux / Unix / MACOSX: compilation from source
 
 The build system is `cmake`. Install the library with
 the standard sequence:
 ```
 cmake .
 make
@@ -58,14 +40,15 @@
 By default optimised release libraries are generated.
 
 ### Windows
 
 Under windows only the static library is generated which
 should be used for your code development.
 
+For example for Visual Studio 2019 you write:
 ```
 cmake -G "Visual Studio 16 2019" -A x64 .
 ```
 and then start Visual C++ and compile it. Usually
 you want to compile both the release and debug
 libraries because they are not compatible to each
 other under Windows.
@@ -74,33 +57,30 @@
 
 The subdirectory `firj` contains an Android project. Load
 it into Android studio and build it either as a release
 or debug binary. This generates an Android aar which you
 import into your project. See the `InstrumentedTest.java`
 for an instructional example.
 
-The pre-compiled libraries are here:
-```Firj/firj/build/outputs/aar/firj-*.aar```
-
 ### Python
 
 #### Installation from the python package index (PyPi)
 
 Windows / Linux / Mac
 ```
-    pip3 install fir1
+pip install fir1
 ```
 under Windows it might be just `pip` for python3.
 
 
 #### Installation from source
 
 Windows / Linux / Mac: make sure that you have swig and a C++ compiler installed. Then type:
 ```
-    python3 setup.py install
+python setup.py install
 ```
 
 
 ## How to use it
 
 ### cmake
 
@@ -131,46 +111,39 @@
 # Sampling rate
 fs = 1000
 # bandstop between 45 and 55 Hz:
 f1 = 45
 f2 = 55
 b = signal.firwin(999,[f1/fs*2,f2/fs*2])
 ```
-For fixed point you need to scale up the coefficients,
-for example by 15 bits: b*32768.
 
 #### octave/MATLAB:
 ```
 octave:1> h=fir1(100,0.1);
 ```
 which creates the coefficients of a lowpass filter with 100 taps
 and normalised cutoff 0.1 to Nyquist.
 
-Again, for fixed point "h" needs to be scaled.
-
 ### Initialisation
 
 #### C++ floating point FIR filter:
 ```
 Fir1 fir("h.dat");
 ```
 or import the coefficients as a const double array:
 ```
 Fir1 fir(coefficients)
 ```
 there is also an option to import a non-const array (for example
-generated with the ifft) and using std::vector.
-
-#### C++ integer FIR filter:
+generated with the ifft) and using std::vector. You can also
+create a moving average filter by initialising all coefficients
+with a constant value:
 ```
-Fir1fixed fir("h_fixed.dat",12);
+Fir1 moving_average(100,1.0/100);
 ```
-where the coefficients have been scaled up by 2^12 and the
-filter will scale them down by this amount (with the help of
-a bitshift operation).
 
 #### JAVA:
 ```
 Fir1 fir = new Fir1(coeff);
 ```
 where `coeff` is an array of double precision coefficients
 and returns the fir filter class.
@@ -183,19 +156,14 @@
 ### Realtime filtering
 
 #### C++ double:
 ```
 double b = fir.filter(a);
 ```
 
-#### C++ integer:
-```
-int b = fir.filter(a);
-```
-
 #### JAVA:
 ```
 double b = fir.filter(a)
 ```
 
 #### Python
 ```
@@ -302,27 +270,24 @@
 ### JAVA/Python
 
 The commands under JAVA and Python are identical to C++.
 
 
 ## Demos
 Demo programs are in the "demo" directory which show how to use the
-filters for both floating point and fixed point.
+filter.
 1. `firdemo` sends an impulse into the filter and you should see the impulse
 response at its output.
-2. `fixeddemo` filters an example ECG with 50Hz noise. The coefficients
-are 12 bit and you can generate them either with OCTAVE/MATLAB or Python.
-The scripts are also provided.
-3. `lmsdemo` filters out 50Hz noise from an ECG with the help of
+2. `lmsdemo` filters out 50Hz noise from an ECG with the help of
 adaptive filtering by using the 50Hz powerline frequency as the input
 to the filter. This can be replaced by any reference artefact signal
 or signal which is correlated with the artefact.
-4. JAVA has an `InstrumentedTest` which filters both a delta pulse and
+3. JAVA has an `InstrumentedTest` which filters both a delta pulse and
 a step function.
-5. filter_ecg.py performs the filtering of an ECG in python using
+4. filter_ecg.py performs the filtering of an ECG in python using
 the fir1 python module which in turn calls internally the C++ functions.
 
 ## C++ documentation
 
 The doxygen generated documentation can be found here:
 
  - Online: http://berndporr.github.io/fir1/index.html
```

### Comparing `fir1-1.7.1.1/README_py.rst` & `fir1-1.8.0.0/README_py.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 Square (NLMS) algorithm.
 
 Installation
 ============
 
 Install the python package with pip::
 
-    pip3 install fir1
+    pip install fir1
 
 You can also install from source::
 
     git clone https://github.com/berndporr/fir1
     cd fir1
-    python3 setup.py install
+    python setup.py install
 
 
 Usage
 =====
 
 Realtime filtering
 ------------------
```

### Comparing `fir1-1.7.1.1/fir1.egg-info/PKG-INFO` & `fir1-1.8.0.0/fir1.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,111 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: fir1
-Version: 1.7.1.1
+Version: 1.8.0.0
 Summary: Efficient FIR realtime filter
 Home-page: https://github.com/berndporr/fir1
 Author: Bernd Porr
 Author-email: mail@berndporr.me.uk
 License: MIT
-Description: ====
-        Fir1
-        ====
-        
-        An efficient Finite Impulse Response (FIR) filter class
-        written in C++ with python wrapper.
-        
-        Adaptive filtering is also implemented using the Least Mean 
-        Square (LMS) or Normalised Least Mean
-        Square (NLMS) algorithm.
-        
-        Installation
-        ============
-        
-        Install the python package with pip::
-        
-            pip3 install fir1
-        
-        You can also install from source::
-        
-            git clone https://github.com/berndporr/fir1
-            cd fir1
-            python3 setup.py install
-        
-        
-        Usage
-        =====
-        
-        Realtime filtering
-        ------------------
-        
-        The filter is a realtime filter which receives samples
-        one by one so it can process data as it arrives from
-        an ADC converter. This is simulated here with the for loop::
-        
-            import fir1
-            b = signal.firwin(999,0.1)
-            f = fir1.Fir1(b)
-            for i in range(len(noisy_signal)):
-                clean_signal[i] = f.filter(noisy_signal[i])
-        
-        The constructor ``Fir1()`` receives the filter coefficients 
-        (= impulse response) and then filtering is performed 
-        with the method ``filter()``.
-        
-        
-        LMS adaptive filter
-        -------------------
-        
-        The file `lms_50Hz_ecg_filter.py` removes 50Hz from 
-        an ECG with the help of the lms filter. 
-        The filter learns its own frequency response from a
-        reference 50Hz sine wave::
-        
-            f = fir1.Fir1(NTAPS)
-            f.setLearningRate(LEARNING_RATE);
-        
-            y= np.empty(len(ecg))
-            for i in range(len(ecg)):
-                ref_noise = np.sin(2.0 * np.pi / 20.0 * i);
-                canceller = f.filter(ref_noise)
-                output_signal = ecg[i] - canceller
-                f.lms_update(output_signal)
-                y[i] = output_signal
-        
-        You can query the filter coefficients using getCoeff.
-        This is most useful to obtain the kernel of a trained
-        adaptive filter::
-        
-                >>> from fir1 import Fir1
-                >>> fir = Fir1([.25, -.5, 1, -.5, .25])
-                >>> fir.getCoeff()
-                array([ 0.25, -0.5 ,  1.  , -0.5 ,  0.25])
-        
-        You may override the length of array to return and
-        the result will be zero-padded. Specifying too small an array
-        causes an exception to be raised::
-        
-                >>> fir.getCoeff(8)
-                array([ 0.25, -0.5 ,  1.  , -0.5 ,  0.25,  0.  ,  0.  ,  0.  ])
-                >>> fir.getCoeff(3)
-                Traceback (most recent call last):
-                File "<stdin>", line 1, in <module>
-                File ".../fir1.py", line 97, in getCoeff
-                return _fir1.Fir1_getCoeff(self, *args)
-                RuntimeError: Fir1: target of getCoeff: too many weights to copy into target
-        
-        
-        Both the demo file and an explanation how the LMS
-        filter works can be found on the homepage of the
-        project:
-        
-        https://github.com/berndporr/fir1
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
+License-File: COPYING
+License-File: AUTHORS
+
+====
+Fir1
+====
+
+An efficient Finite Impulse Response (FIR) filter class
+written in C++ with python wrapper.
+
+Adaptive filtering is also implemented using the Least Mean 
+Square (LMS) or Normalised Least Mean
+Square (NLMS) algorithm.
+
+Installation
+============
+
+Install the python package with pip::
+
+    pip install fir1
+
+You can also install from source::
+
+    git clone https://github.com/berndporr/fir1
+    cd fir1
+    python setup.py install
+
+
+Usage
+=====
+
+Realtime filtering
+------------------
+
+The filter is a realtime filter which receives samples
+one by one so it can process data as it arrives from
+an ADC converter. This is simulated here with the for loop::
+
+    import fir1
+    b = signal.firwin(999,0.1)
+    f = fir1.Fir1(b)
+    for i in range(len(noisy_signal)):
+        clean_signal[i] = f.filter(noisy_signal[i])
+
+The constructor ``Fir1()`` receives the filter coefficients 
+(= impulse response) and then filtering is performed 
+with the method ``filter()``.
+
+
+LMS adaptive filter
+-------------------
+
+The file `lms_50Hz_ecg_filter.py` removes 50Hz from 
+an ECG with the help of the lms filter. 
+The filter learns its own frequency response from a
+reference 50Hz sine wave::
+
+    f = fir1.Fir1(NTAPS)
+    f.setLearningRate(LEARNING_RATE);
+
+    y= np.empty(len(ecg))
+    for i in range(len(ecg)):
+        ref_noise = np.sin(2.0 * np.pi / 20.0 * i);
+        canceller = f.filter(ref_noise)
+        output_signal = ecg[i] - canceller
+        f.lms_update(output_signal)
+        y[i] = output_signal
+
+You can query the filter coefficients using getCoeff.
+This is most useful to obtain the kernel of a trained
+adaptive filter::
+
+        >>> from fir1 import Fir1
+        >>> fir = Fir1([.25, -.5, 1, -.5, .25])
+        >>> fir.getCoeff()
+        array([ 0.25, -0.5 ,  1.  , -0.5 ,  0.25])
+
+You may override the length of array to return and
+the result will be zero-padded. Specifying too small an array
+causes an exception to be raised::
+
+        >>> fir.getCoeff(8)
+        array([ 0.25, -0.5 ,  1.  , -0.5 ,  0.25,  0.  ,  0.  ,  0.  ])
+        >>> fir.getCoeff(3)
+        Traceback (most recent call last):
+        File "<stdin>", line 1, in <module>
+        File ".../fir1.py", line 97, in getCoeff
+        return _fir1.Fir1_getCoeff(self, *args)
+        RuntimeError: Fir1: target of getCoeff: too many weights to copy into target
+
+
+Both the demo file and an explanation how the LMS
+filter works can be found on the homepage of the
+project:
+
+https://github.com/berndporr/fir1
+
+
```

### Comparing `fir1-1.7.1.1/fir1.i` & `fir1-1.8.0.0/fir1.i`

 * *Files 2% similar despite different names*

```diff
@@ -38,11 +38,11 @@
                 # Set the number of taps to return from the number of weights.
                 return $action(self, self.getTaps())
         else :
                 # If any other arguments are supplied, pass them through to the C++ library.
                 return $action(self, *args)
 %}
 
-%apply (double* IN_ARRAY1, int DIM1) {(double *coefficients, unsigned number_of_taps)};
+%apply (double* IN_ARRAY1, int DIM1) {(const double *coefficients, const unsigned number_of_taps)};
 %apply (double* ARGOUT_ARRAY1, int DIM1) {(double *coeff_data, unsigned number_of_taps)};
 
 %include "Fir1.h"
```

### Comparing `fir1-1.7.1.1/fir1.py` & `fir1-1.8.0.0/fir1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This file was automatically generated by SWIG (http://www.swig.org).
-# Version 4.0.1
+# Version 4.0.2
 #
 # Do not make changes to this file unless you know what you are doing--modify
 # the SWIG interface file instead.
 
 from sys import version_info as _swig_python_version_info
 if _swig_python_version_info < (2, 7, 0):
     raise RuntimeError("Python 2.7 or later required")
@@ -94,14 +94,17 @@
                     return _fir1.Fir1_getCoeff(self, self.getTaps())
             else :
     # If any other arguments are supplied, pass them through to the C++ library.
                     return _fir1.Fir1_getCoeff(self, *args)
 
 
 
+    def setCoeff(self, coeff_data: "double const *", number_of_taps: "unsigned int const") -> "void":
+        return _fir1.Fir1_setCoeff(self, coeff_data, number_of_taps)
+
     def getTaps(self) -> "unsigned int":
         return _fir1.Fir1_getTaps(self)
 
     def getTapInputPower(self) -> "double":
         return _fir1.Fir1_getTapInputPower(self)
 
 # Register Fir1 in _fir1:
```

### Comparing `fir1-1.7.1.1/numpy.i` & `fir1-1.8.0.0/numpy.i`

 * *Files identical despite different names*

### Comparing `fir1-1.7.1.1/setup.py` & `fir1-1.8.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 			    extra_compile_args=['/DWIN32_LEAN_AND_MEAN'],
                             swig_opts=['-c++','-py3'],
 			    include_dirs=[numpy.get_include()],
 	                       )
 
 						   
 setup (name = 'fir1',
-       version = '1.7.1.1',
+       version = '1.8.0.0',
        author      = "Bernd Porr",
        author_email = "mail@berndporr.me.uk",
        url = "https://github.com/berndporr/fir1",
        description = 'Efficient FIR realtime filter',
        long_description=read('README_py.rst'),
        ext_modules = [fir1_module],
        py_modules = ["fir1"],
```

