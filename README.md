# Yulp_business
{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 1,
   "id": "6b22a777",
   "metadata": {},
   "outputs": [],
   "source": [
    "import numpy as np"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "id": "321e6fd3",
   "metadata": {},
   "outputs": [],
   "source": [
    "a = [2, 5, 7]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "id": "3f6b4e55",
   "metadata": {},
   "outputs": [],
   "source": [
    "b = [3, 12, 27]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "id": "3334079d",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[2, 5, 7, 3, 12, 27]"
      ]
     },
     "execution_count": 4,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "a+b"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "id": "400abe43",
   "metadata": {},
   "outputs": [],
   "source": [
    "c = [m+n for m, n in zip(a,b)]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "id": "1da29ce4",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[5, 17, 34]"
      ]
     },
     "execution_count": 6,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "c"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 7,
   "id": "5f8525c9",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "14"
      ]
     },
     "execution_count": 7,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "sum(a)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 8,
   "id": "c3cd1fbc",
   "metadata": {},
   "outputs": [],
   "source": [
    "np_a = np.array(a)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "id": "a598c170",
   "metadata": {},
   "outputs": [],
   "source": [
    "np_b = np.array(b)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 11,
   "id": "f4c2d368",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([ 5, 17, 34])"
      ]
     },
     "execution_count": 11,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_a + np_b"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 12,
   "id": "53ea6f88",
   "metadata": {},
   "outputs": [],
   "source": [
    "p = np.array([1,2,\"abc\"])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 13,
   "id": "7596c7fc",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array(['1', '2', 'abc'], dtype='<U11')"
      ]
     },
     "execution_count": 13,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "p"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 14,
   "id": "2427f9d5",
   "metadata": {},
   "outputs": [
    {
     "ename": "UFuncTypeError",
     "evalue": "ufunc 'add' did not contain a loop with signature matching types (dtype('<U11'), dtype('<U11')) -> dtype('<U11')",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mUFuncTypeError\u001b[0m                            Traceback (most recent call last)",
      "\u001b[1;32mC:\\Users\\BHAVIK~1.GAN\\AppData\\Local\\Temp/ipykernel_28232/3599995278.py\u001b[0m in \u001b[0;36m<module>\u001b[1;34m\u001b[0m\n\u001b[1;32m----> 1\u001b[1;33m \u001b[0mp\u001b[0m\u001b[1;33m+\u001b[0m \u001b[0mnp_a\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[1;31mUFuncTypeError\u001b[0m: ufunc 'add' did not contain a loop with signature matching types (dtype('<U11'), dtype('<U11')) -> dtype('<U11')"
     ]
    }
   ],
   "source": [
    "p+ np_a"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 15,
   "id": "9a9fd1eb",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "7"
      ]
     },
     "execution_count": 15,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_a.max()"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 16,
   "id": "6b20d0cb",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "4.666666666666667"
      ]
     },
     "execution_count": 16,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_a.mean()"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 17,
   "id": "cdb4fb5a",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([1., 1., 1.])"
      ]
     },
     "execution_count": 17,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np.ones(3)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 18,
   "id": "2f91e614",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([0., 0., 0.])"
      ]
     },
     "execution_count": 18,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np.zeros(3)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 19,
   "id": "0f506dcf",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([2., 5., 7.])"
      ]
     },
     "execution_count": 19,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_a*np.ones(3)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 20,
   "id": "bddabd58",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([ 6, 15, 21])"
      ]
     },
     "execution_count": 20,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_a*[3]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 21,
   "id": "bcfb05a5",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([ 4.4, 11. , 15.4])"
      ]
     },
     "execution_count": 21,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_a*np.array([2.2])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 22,
   "id": "5c2dbd16",
   "metadata": {},
   "outputs": [
    {
     "ename": "ValueError",
     "evalue": "operands could not be broadcast together with shapes (3,) (2,) ",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mValueError\u001b[0m                                Traceback (most recent call last)",
      "\u001b[1;32mC:\\Users\\BHAVIK~1.GAN\\AppData\\Local\\Temp/ipykernel_28232/3306110916.py\u001b[0m in \u001b[0;36m<module>\u001b[1;34m\u001b[0m\n\u001b[1;32m----> 1\u001b[1;33m \u001b[0mnp_a\u001b[0m\u001b[1;33m*\u001b[0m\u001b[0mnp\u001b[0m\u001b[1;33m.\u001b[0m\u001b[0marray\u001b[0m\u001b[1;33m(\u001b[0m\u001b[1;33m[\u001b[0m\u001b[1;36m2.2\u001b[0m\u001b[1;33m,\u001b[0m\u001b[1;36m3.2\u001b[0m\u001b[1;33m]\u001b[0m\u001b[1;33m)\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[1;31mValueError\u001b[0m: operands could not be broadcast together with shapes (3,) (2,) "
     ]
    }
   ],
   "source": [
    "np_a*np.array([2.2,3.2])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 23,
   "id": "447c664f",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "5"
      ]
     },
     "execution_count": 23,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_a[1]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 24,
   "id": "121df768",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([5, 7])"
      ]
     },
     "execution_count": 24,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_a[1:]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 25,
   "id": "b57d393a",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([2, 5])"
      ]
     },
     "execution_count": 25,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_a[0:2]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 27,
   "id": "20a1d70e",
   "metadata": {},
   "outputs": [],
   "source": [
    "np_2d = np.array([[1,2],[3,4]])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 28,
   "id": "742f24d3",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "10"
      ]
     },
     "execution_count": 28,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d.sum()"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 29,
   "id": "bc4a4677",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([4, 6])"
      ]
     },
     "execution_count": 29,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d.sum(axis=0)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 30,
   "id": "82349735",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([3, 7])"
      ]
     },
     "execution_count": 30,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d.sum(axis=1)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 31,
   "id": "05b1b764",
   "metadata": {},
   "outputs": [
    {
     "ename": "TypeError",
     "evalue": "'numpy.ndarray' object is not callable",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mTypeError\u001b[0m                                 Traceback (most recent call last)",
      "\u001b[1;32mC:\\Users\\BHAVIK~1.GAN\\AppData\\Local\\Temp/ipykernel_28232/4106328631.py\u001b[0m in \u001b[0;36m<module>\u001b[1;34m\u001b[0m\n\u001b[1;32m----> 1\u001b[1;33m \u001b[0mnp_2d\u001b[0m\u001b[1;33m.\u001b[0m\u001b[0mT\u001b[0m\u001b[1;33m(\u001b[0m\u001b[1;33m)\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[1;31mTypeError\u001b[0m: 'numpy.ndarray' object is not callable"
     ]
    }
   ],
   "source": [
    "np_2d.T()"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 32,
   "id": "c0bfe2d8",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1, 3],\n",
       "       [2, 4]])"
      ]
     },
     "execution_count": 32,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d.T"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 34,
   "id": "9815b626",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1., 1.],\n",
       "       [1., 1.]])"
      ]
     },
     "execution_count": 34,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np.ones([2,2])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 36,
   "id": "a2a19ba4",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1., 0.],\n",
       "       [0., 1.]])"
      ]
     },
     "execution_count": 36,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np.eye(2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 37,
   "id": "57213d72",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1, 2],\n",
       "       [3, 4]])"
      ]
     },
     "execution_count": 37,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 38,
   "id": "54583779",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[2., 3.],\n",
       "       [4., 5.]])"
      ]
     },
     "execution_count": 38,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d+np.ones([2,2])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 39,
   "id": "87eadd94",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[2., 3.],\n",
       "       [4., 5.]])"
      ]
     },
     "execution_count": 39,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d+np.ones(2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 41,
   "id": "8d0ca5db",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[2., 3.],\n",
       "       [4., 5.]])"
      ]
     },
     "execution_count": 41,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d+np.ones([2,1])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 43,
   "id": "e19aacc8",
   "metadata": {},
   "outputs": [],
   "source": [
    "np_dotp = np_2d.dot(np.array([[1,10,100],[1000,100,10]]))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 44,
   "id": "91cf6331",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[2001,  210,  120],\n",
       "       [4003,  430,  340]])"
      ]
     },
     "execution_count": 44,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_dotp"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 45,
   "id": "98ae8064",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "210"
      ]
     },
     "execution_count": 45,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_dotp[0,1]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 46,
   "id": "cbc1b40b",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[4003,  430,  340]])"
      ]
     },
     "execution_count": 46,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_dotp[1:3]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 47,
   "id": "45186705",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([2001, 4003])"
      ]
     },
     "execution_count": 47,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_dotp[0:2,0]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 48,
   "id": "b1c39f6a",
   "metadata": {},
   "outputs": [],
   "source": [
    "np_rs = np.array([1,2,3,4,5,6])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 49,
   "id": "f2feaa22",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([1, 2, 3, 4, 5, 6])"
      ]
     },
     "execution_count": 49,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_rs"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 50,
   "id": "9800a502",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1, 2, 3],\n",
       "       [4, 5, 6]])"
      ]
     },
     "execution_count": 50,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_rs.reshape(2,3)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 51,
   "id": "0dae4fcf",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1, 2],\n",
       "       [3, 4],\n",
       "       [5, 6]])"
      ]
     },
     "execution_count": 51,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_rs.reshape(3,2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 52,
   "id": "d556ffed",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1, 2],\n",
       "       [3, 4],\n",
       "       [5, 6]])"
      ]
     },
     "execution_count": 52,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_rs.reshape(3,-1)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 53,
   "id": "db952d1d",
   "metadata": {},
   "outputs": [
    {
     "ename": "ValueError",
     "evalue": "cannot reshape array of size 6 into shape (4,newaxis)",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mValueError\u001b[0m                                Traceback (most recent call last)",
      "\u001b[1;32mC:\\Users\\BHAVIK~1.GAN\\AppData\\Local\\Temp/ipykernel_28232/2065866566.py\u001b[0m in \u001b[0;36m<module>\u001b[1;34m\u001b[0m\n\u001b[1;32m----> 1\u001b[1;33m \u001b[0mnp_rs\u001b[0m\u001b[1;33m.\u001b[0m\u001b[0mreshape\u001b[0m\u001b[1;33m(\u001b[0m\u001b[1;36m4\u001b[0m\u001b[1;33m,\u001b[0m\u001b[1;33m-\u001b[0m\u001b[1;36m1\u001b[0m\u001b[1;33m)\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[1;31mValueError\u001b[0m: cannot reshape array of size 6 into shape (4,newaxis)"
     ]
    }
   ],
   "source": [
    "np_rs.reshape(4,-1)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 54,
   "id": "b53c8a9c",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1, 2, 3],\n",
       "       [4, 5, 6]])"
      ]
     },
     "execution_count": 54,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_rs.reshape(2,-1)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 56,
   "id": "d1d8816c",
   "metadata": {},
   "outputs": [
    {
     "ename": "ValueError",
     "evalue": "cannot reshape array of size 6 into shape (2,2,newaxis)",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mValueError\u001b[0m                                Traceback (most recent call last)",
      "\u001b[1;32mC:\\Users\\BHAVIK~1.GAN\\AppData\\Local\\Temp/ipykernel_28232/3633391268.py\u001b[0m in \u001b[0;36m<module>\u001b[1;34m\u001b[0m\n\u001b[1;32m----> 1\u001b[1;33m \u001b[0mnp_rs\u001b[0m\u001b[1;33m.\u001b[0m\u001b[0mreshape\u001b[0m\u001b[1;33m(\u001b[0m\u001b[1;36m2\u001b[0m\u001b[1;33m,\u001b[0m\u001b[1;36m2\u001b[0m\u001b[1;33m,\u001b[0m\u001b[1;33m-\u001b[0m\u001b[1;36m1\u001b[0m\u001b[1;33m)\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[1;31mValueError\u001b[0m: cannot reshape array of size 6 into shape (2,2,newaxis)"
     ]
    }
   ],
   "source": [
    "np_rs.reshape(2,2,-1)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 57,
   "id": "47ded2fd",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1, 2, 3],\n",
       "       [4, 5, 6]])"
      ]
     },
     "execution_count": 57,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_rs.reshape(-1,3)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 58,
   "id": "f552302c",
   "metadata": {},
   "outputs": [
    {
     "ename": "TypeError",
     "evalue": "'module' object is not callable",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mTypeError\u001b[0m                                 Traceback (most recent call last)",
      "\u001b[1;32mC:\\Users\\BHAVIK~1.GAN\\AppData\\Local\\Temp/ipykernel_28232/4177975657.py\u001b[0m in \u001b[0;36m<module>\u001b[1;34m\u001b[0m\n\u001b[1;32m----> 1\u001b[1;33m \u001b[0mnp\u001b[0m\u001b[1;33m.\u001b[0m\u001b[0mrandom\u001b[0m\u001b[1;33m(\u001b[0m\u001b[1;36m2\u001b[0m\u001b[1;33m)\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[1;31mTypeError\u001b[0m: 'module' object is not callable"
     ]
    }
   ],
   "source": [
    "np.random(2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 59,
   "id": "41fb9382",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([0.43365602, 0.67705795])"
      ]
     },
     "execution_count": 59,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np.random.random(2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 60,
   "id": "153b11b5",
   "metadata": {},
   "outputs": [
    {
     "ename": "ModuleNotFoundError",
     "evalue": "No module named 'np'",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mModuleNotFoundError\u001b[0m                       Traceback (most recent call last)",
      "\u001b[1;32mC:\\Users\\BHAVIK~1.GAN\\AppData\\Local\\Temp/ipykernel_28232/450834328.py\u001b[0m in \u001b[0;36m<module>\u001b[1;34m\u001b[0m\n\u001b[1;32m----> 1\u001b[1;33m \u001b[1;32mimport\u001b[0m \u001b[0mnp\u001b[0m\u001b[1;33m.\u001b[0m\u001b[0mrandom\u001b[0m \u001b[1;32mas\u001b[0m \u001b[0mrandom\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[1;31mModuleNotFoundError\u001b[0m: No module named 'np'"
     ]
    }
   ],
   "source": [
    "import np.random as random"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 61,
   "id": "f14c1645",
   "metadata": {},
   "outputs": [],
   "source": [
    "import numpy.random as random"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 62,
   "id": "12b02be0",
   "metadata": {},
   "outputs": [
    {
     "ename": "TypeError",
     "evalue": "'module' object is not callable",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mTypeError\u001b[0m                                 Traceback (most recent call last)",
      "\u001b[1;32mC:\\Users\\BHAVIK~1.GAN\\AppData\\Local\\Temp/ipykernel_28232/804514816.py\u001b[0m in \u001b[0;36m<module>\u001b[1;34m\u001b[0m\n\u001b[1;32m----> 1\u001b[1;33m \u001b[0mrandom\u001b[0m\u001b[1;33m(\u001b[0m\u001b[1;36m2\u001b[0m\u001b[1;33m)\u001b[0m\u001b[1;33m\u001b[0m\u001b[1;33m\u001b[0m\u001b[0m\n\u001b[0m",
      "\u001b[1;31mTypeError\u001b[0m: 'module' object is not callable"
     ]
    }
   ],
   "source": [
    "random(2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 63,
   "id": "29fd7c12",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([0.26399133, 0.7125254 ])"
      ]
     },
     "execution_count": 63,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.random(2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 65,
   "id": "50e77f01",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[0.30526688, 0.41513002],\n",
       "       [0.598052  , 0.11485611],\n",
       "       [0.0684223 , 0.54712717]])"
      ]
     },
     "execution_count": 65,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.random([3,2])"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 66,
   "id": "5be6ad52",
   "metadata": {},
   "outputs": [],
   "source": [
    "import numpy.linalg as la"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 67,
   "id": "c91badea",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[-2. ,  1. ],\n",
       "       [ 1.5, -0.5]])"
      ]
     },
     "execution_count": 67,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "la.inv(np_2d)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 68,
   "id": "190d9150",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "(array([-0.37228132,  5.37228132]),\n",
       " array([[-0.82456484, -0.41597356],\n",
       "        [ 0.56576746, -0.90937671]]))"
      ]
     },
     "execution_count": 68,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "la.eig(np_2d)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 70,
   "id": "2e922a01",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "(array([[-0.40455358, -0.9145143 ],\n",
       "        [-0.9145143 ,  0.40455358]]),\n",
       " array([5.4649857 , 0.36596619]),\n",
       " array([[-0.57604844, -0.81741556],\n",
       "        [ 0.81741556, -0.57604844]]))"
      ]
     },
     "execution_count": 70,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "la.svd(np_2d)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 71,
   "id": "a441edcb",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[-2. ,  1. ],\n",
       "       [ 1.5, -0.5]])"
      ]
     },
     "execution_count": 71,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "la.pinv(np_2d)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 75,
   "id": "0b049bfc",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1.91814336, 3.3888604 , 1.73449056],\n",
       "       [4.35126763, 2.85394498, 4.83614907]])"
      ]
     },
     "execution_count": 75,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.rand(2,3)*5"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 74,
   "id": "6c0ec0e3",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[-1.23473641,  1.20362352, -0.0691662 ],\n",
       "       [ 0.0334294 ,  1.00109125, -0.22592634]])"
      ]
     },
     "execution_count": 74,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.randn(2,3)"
   ]
  },
  {
   "cell_type": "raw",
   "id": "9a427a24",
   "metadata": {},
   "source": [
    "random.randint(-2,5,3)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 76,
   "id": "2a7e897a",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([ 1, -1, -2,  2,  0])"
      ]
     },
     "execution_count": 76,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.randint(-2,3,5)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 77,
   "id": "52b331b2",
   "metadata": {},
   "outputs": [],
   "source": [
    "random.shuffle(np_rs)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 78,
   "id": "cee749c4",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([3, 6, 4, 1, 2, 5])"
      ]
     },
     "execution_count": 78,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_rs"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 79,
   "id": "53d0e965",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([1, 6])"
      ]
     },
     "execution_count": 79,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.choice(np_rs, 2)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 80,
   "id": "60f3d510",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "5"
      ]
     },
     "execution_count": 80,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.binomial(20,0.3)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 81,
   "id": "f581cef6",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([ 5,  8,  2,  7,  7, 10,  4])"
      ]
     },
     "execution_count": 81,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.binomial(20, 0.3, 7)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 82,
   "id": "316e609a",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([0.13372559, 0.62232793, 1.1424338 , 0.36568844])"
      ]
     },
     "execution_count": 82,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.exponential(0.7,4)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "c3c3da6e",
   "metadata": {},
   "outputs": [],
   "source": [
    "%%time\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 83,
   "id": "0df740eb",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([-13.16651465,  -0.12575013,  -1.52670445])"
      ]
     },
     "execution_count": 83,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.normal(-5,12,3)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 84,
   "id": "ae4df0fe",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([-13.86959627,  -6.28421112,  -2.89562533,  -2.56350521,\n",
       "         3.03949534,  -9.1472225 ,   6.53402689])"
      ]
     },
     "execution_count": 84,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "random.logistic(-2,4,7)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 85,
   "id": "197bd554",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "(2, 2)"
      ]
     },
     "execution_count": 85,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d.shape"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 86,
   "id": "2f09cee7",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "dtype('int32')"
      ]
     },
     "execution_count": 86,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np_2d.dtype"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 87,
   "id": "68058276",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "numpy.ndarray"
      ]
     },
     "execution_count": 87,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "type(np_2d)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 90,
   "id": "188f8626",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1., 1.],\n",
       "       [1., 1.]])"
      ]
     },
     "execution_count": 90,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np.vstack(np.ones([2,2]))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 94,
   "id": "1c81dfac",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1., 2.],\n",
       "       [3., 4.],\n",
       "       [1., 1.],\n",
       "       [1., 1.]])"
      ]
     },
     "execution_count": 94,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np.vstack((np_2d,np.ones([2,2])))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 95,
   "id": "190dfbcf",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "array([[1., 2., 1., 1.],\n",
       "       [3., 4., 1., 1.]])"
      ]
     },
     "execution_count": 95,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "np.hstack((np_2d,np.ones([2,2])))"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 96,
   "id": "8cac5e59",
   "metadata": {},
   "outputs": [],
   "source": [
    "N=10000000\n",
    "x=list(range(N))\n",
    "y=list(range(N)) \n",
    "z=[]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 97,
   "id": "eaf5a569",
   "metadata": {},
   "outputs": [],
   "source": [
    "np_x = np.array(x)\n",
    "np_y = np.array(y)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 100,
   "id": "815dcb98",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Wall time: 1.96 s\n"
     ]
    }
   ],
   "source": [
    "%%time\n",
    "for i in range(len(x)):\n",
    "    z.append(x[i]+y[i])\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 99,
   "id": "42adb9fa",
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Wall time: 32.9 ms\n"
     ]
    }
   ],
   "source": [
    "%%time\n",
    "np_z = np_x+np_y"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "b9396fa1",
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
