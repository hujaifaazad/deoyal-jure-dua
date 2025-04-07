# deoyal-jure-dua
ইসলামিক ওয়াল আর্ট এবং ক্যালিগ্রাফি প্রোডাক্ট
import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";

export default function Home() {
  return (
    <main className="min-h-screen bg-gradient-to-b from-white to-green-50 p-4">
      <header className="text-center py-6">
        <h1 className="text-3xl md:text-5xl font-bold text-green-800">দেয়াল জুড়ে দোয়া</h1>
        <p className="text-green-600 mt-2 text-lg">আপনার ঘর হোক জান্নাতের প্রতিচ্ছবি</p>
      </header>

      <section className="grid md:grid-cols-2 lg:grid-cols-3 gap-4 mt-8">
        {[1, 2, 3, 4, 5, 6].map((item) => (
          <Card key={item} className="hover:shadow-lg transition-all">
            <img
              src={`/art/sample${item}.jpg`}
              alt={`আর্টওয়ার্ক ${item}`}
              className="rounded-t-xl h-60 w-full object-cover"
            />
            <CardContent className="p-4">
              <h2 className="text-xl font-semibold text-green-700">ইসলামিক ওয়াল আর্ট {item}</h2>
              <p className="text-sm text-gray-600 mt-1">আয়াতুল কুরসী সহ আকর্ষণীয় ডিজাইন</p>
              <Button className="mt-4 w-full bg-green-700 hover:bg-green-800 text-white">
                অর্ডার করুন
              </Button>
            </CardContent>
          </Card>
        ))}
      </section>

      <section className="mt-16 bg-green-100 p-6 rounded-xl max-w-3xl mx-auto">
        <h2 className="text-2xl font-bold text-green-800 mb-4 text-center">আমাদের সম্পর্কে</h2>
        <p className="text-gray-700 leading-relaxed">
          'দেয়াল জুড়ে দোয়া' এমন একটি উদ্যোগ যা ইসলামিক কলিগ্রাফি এবং আয়াতের মাধ্যমে আপনার ঘরে আনে পবিত্রতা, শান্তি এবং বারাকাহ। আমরা বিশ্বাস করি, প্রতিটি দেয়ালই হতে পারে আল্লাহর স্মরণে সাজানো একটি স্থান।
        </p>
      </section>

      <section className="mt-12 max-w-xl mx-auto bg-white p-6 rounded-xl shadow-md">
        <h2 className="text-xl font-semibold text-green-700 mb-4 text-center">অর্ডার করুন</h2>
        <form className="space-y-4">
          <input
            type="text"
            placeholder="আপনার নাম"
            className="w-full p-2 border border-green-300 rounded"
          />
          <input
            type="text"
            placeholder="মোবাইল নম্বর"
            className="w-full p-2 border border-green-300 rounded"
          />
          <textarea
            placeholder="আপনার ঠিকানা ও প্রোডাক্ট নাম লিখুন"
            className="w-full p-2 border border-green-300 rounded"
          ></textarea>
          <Button className="w-full bg-green-700 hover:bg-green-800 text-white">
            অর্ডার সাবমিট করুন
          </Button>
        </form>
      </section>

      <footer className="text-center text-sm text-gray-600 mt-12 py-6">
        © ২০২৫ দেয়াল জুড়ে দোয়া | ইসলামিক ওয়াল আর্ট বাংলাদেশ
      </footer>
    </main>
  );
}

